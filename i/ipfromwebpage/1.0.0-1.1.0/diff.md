# Comparing `tmp/ipfromwebpage-1.0.0.tar.gz` & `tmp/ipfromwebpage-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfromwebpage-1.0.0.tar", last modified: Tue Jan 21 00:55:36 2020, max compression
+gzip compressed data, was "ipfromwebpage-1.1.0.tar", max compression
```

## Comparing `ipfromwebpage-1.0.0.tar` & `ipfromwebpage-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1079 2020-01-21 00:55:13.557218 ipfromwebpage-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     1273 2020-01-21 00:55:13.557218 ipfromwebpage-1.0.0/README.md
--rw-r--r--   0        0        0       97 2020-01-21 00:55:13.557218 ipfromwebpage-1.0.0/ipfromwebpage/__init__.py
--rw-r--r--   0        0        0     5350 2020-01-21 00:55:13.557218 ipfromwebpage-1.0.0/ipfromwebpage/ipfromwebpage.py
--rw-r--r--   0        0        0     1015 2020-01-21 00:55:13.557218 ipfromwebpage-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2161 2020-01-21 00:55:36.435167 ipfromwebpage-1.0.0/setup.py
--rw-r--r--   0        0        0     2194 2020-01-21 00:55:36.435468 ipfromwebpage-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-02-06 15:15:00.570694 ipfromwebpage-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     1201 2023-04-24 18:33:48.645593 ipfromwebpage-1.1.0/README.md
+-rw-r--r--   0        0        0       97 2023-02-06 15:15:00.571287 ipfromwebpage-1.1.0/ipfromwebpage/__init__.py
+-rw-r--r--   0        0        0     4772 2023-04-24 19:32:43.476616 ipfromwebpage-1.1.0/ipfromwebpage/ipfromwebpage.py
+-rw-r--r--   0        0        0     1131 2023-04-24 19:32:43.478537 ipfromwebpage-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 ipfromwebpage-1.1.0/setup.py
+-rw-r--r--   0        0        0     2445 1970-01-01 00:00:00.000000 ipfromwebpage-1.1.0/PKG-INFO
```

### Comparing `ipfromwebpage-1.0.0/LICENSE.md` & `ipfromwebpage-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ipfromwebpage-1.0.0/README.md` & `ipfromwebpage-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 ## ipfromwebpage
 
 [![PyPi](https://img.shields.io/pypi/v/ipfromwebpage.svg)](https://pypi.python.org/pypi/ipfromwebpage)
-[![Build Status](https://travis-ci.org/shepherdjay/ipfromwebpage.svg?branch=master)](https://travis-ci.org/shepherdjay/ipfromwebpage)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/shepherdjay/ipfromwebpage/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/shepherdjay/ipfromwebpage/tree/master)
 [![codecov](https://codecov.io/gh/shepherdjay/ipfromwebpage/branch/master/graph/badge.svg)](https://codecov.io/gh/shepherdjay/ipfromwebpage)
-[![Updates](https://pyup.io/repos/github/shepherdjay/ipfromwebpage/shield.svg)](https://pyup.io/repos/github/shepherdjay/ipfromwebpage/)
 
 ### Summary:
 Takes a webpage and scrapes for IPv4 Addresses. Then prints the IPs. (aggregated where possible)
 
 #### Quickstart:
 
 Install using `pip install ipfromwebpage`
```

### Comparing `ipfromwebpage-1.0.0/ipfromwebpage/ipfromwebpage.py` & `ipfromwebpage-1.1.0/ipfromwebpage/ipfromwebpage.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,140 +5,122 @@
 import sys
 from urllib.parse import urlparse
 from urllib.request import urlopen
 
 import bs4
 import netaddr
 
+IPv4_EXCLUSIONS = netaddr.IPSet([
+        '0.0.0.0/8',
+        '224.0.0.0/3'
+])
+
 
 def check_args(args=None):
     parser = argparse.ArgumentParser(description="IP Webpage Scraper")
     parser.add_argument('url',
                         type=argparse_url_type,
                         help="URL to scrape, must be FQDN ie https://example.com")
     return parser.parse_args(args)
 
 
-def argparse_url_type(url_to_check):
-    """
-    This is a helper function that wires check_args to validate_url
-    :param url_to_check: The URL positional argument passed from argparse
-    :return: Value if okay, otherwise raises argparse exception
-    """
+def argparse_url_type(url_to_check: str) -> str:
+    """This is a helper function that wires check_args to validate_url"""
     result = validate_url(url_to_check)
     if result:
         return url_to_check
     else:
         raise argparse.ArgumentTypeError(
             "{} is an invalid URL, must specify fqdn, ex. https://www.example.com".format(url_to_check))
 
 
-def validate_url(url_arg):
-    """
-    Takes string input and validates url refers to a valid webpage for passing into other functions
-    :param url_arg: URL to check for validation
-    :return: Boolean result of validation check
-    """
+def validate_url(url_arg: str) -> bool:
+    """Takes string input and validates url refers to a valid webpage for passing into other functions"""
     parse = urlparse(url_arg)
     if parse.scheme not in ['http', 'https']:
         return False
     if '.' not in parse.netloc:
         return False
     return True
 
 
-def get_webpage_text(url_input):
-    """
-    Extracts text of webpage and returns
-    :param url_input: Fully-qualified webpage url to get contents of
-    :return: Text of webpage
-    """
+def get_webpage_text(url_input: str) -> str:
+    """Extracts text of webpage and returns"""
     data = bs4.BeautifulSoup(urlopen(url_input), 'html.parser').get_text()
     return data
 
 
-def validate_ip(ip):
-    """
-    Validates if passed string is an ipv4 or ipv6 address or network.
-    :param ip: IP Address as string
-    :return: Boolean Result
-    """
+def validate_ip(ip: str) -> bool:
+    """Validates if passed string is an ipv4 or ipv6 address or network."""
     try:
         if '/' in ip:
             netaddr.IPNetwork(ip)
         else:
             netaddr.IPAddress(ip)
         return True
     except netaddr.AddrFormatError:
         return False
 
 
-def ip_from_string(string):
+def ip_from_string(string: str) -> netaddr.IPSet:
     """
     Takes a string and extracts all valid IP Addresses as a SET of Strings
     Uses the validate_ip helper function to achieve.
-    :param string: Any string of data
-    :return: IP Addresses as a netaddr.IPSet or empty netaddr.IPSet if none found
     """
-    ip_regex = re.compile('(?<!\.)(?:[0-9]{1,3}\.){3}[0-9]{1,3}(?!\.)(?:\/[0-9]{1,2})?')
+    ip_regex = re.compile(r'(?<!\.)(?:[0-9]{1,3}\.){3}[0-9]{1,3}(?!\.)(?:\/[0-9]{1,2})?')
     potential_ips = ip_regex.findall(string)
     valid_ips = []
     for ip in potential_ips:
         if validate_ip(ip) is True:
             valid_ips.append(ip)
-    return netaddr.IPSet(valid_ips)
+    return netaddr.IPSet(valid_ips) - IPv4_EXCLUSIONS
 
 
-def ipv6_from_string(string):
+def ipv6_from_string(string: str) -> netaddr.IPSet:
     """
     Takes a string and extracts all valid IPv6 Addresses as a SET of Strings
     Uses the validate_ip helper function to achieve.
-    :param string: Any string of data
-    :return: IPv6 Addresses as a netaddr.IPSet or empty netaddr.IPSet if none found
     """
 
     ipv6_regex = re.compile(
-        '(?<![a-zA-Z\d\.])((([0-9A-Fa-f]{1,4}:){7}([0-9A-Fa-f]{1,4}|:))|(([0-9A-Fa-f]{1,4}:){6}(:[0-9A-Fa-f]{1,4}|((25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)(\.(25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)){3})|:))|(([0-9A-Fa-f]{1,4}:){5}(((:[0-9A-Fa-f]{1,4}){1,2})|:((25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)(\.(25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)){3})|:))|(([0-9A-Fa-f]{1,4}:){4}(((:[0-9A-Fa-f]{1,4}){1,3})|((:[0-9A-Fa-f]{1,4})?:((25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)(\.(25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)){3}))|:))|(([0-9A-Fa-f]{1,4}:){3}(((:[0-9A-Fa-f]{1,4}){1,4})|((:[0-9A-Fa-f]{1,4}){0,2}:((25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)(\.(25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)){3}))|:))|(([0-9A-Fa-f]{1,4}:){2}(((:[0-9A-Fa-f]{1,4}){1,5})|((:[0-9A-Fa-f]{1,4}){0,3}:((25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)(\.(25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)){3}))|:))|(([0-9A-Fa-f]{1,4}:){1}(((:[0-9A-Fa-f]{1,4}){1,6})|((:[0-9A-Fa-f]{1,4}){0,4}:((25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)(\.(25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)){3}))|:))|(:(((:[0-9A-Fa-f]{1,4}){1,7})|((:[0-9A-Fa-f]{1,4}){0,5}:((25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)(\.(25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)){3}))|:)))(%.+)?(\/[\d][\d]?[\d]?|1([01][0-9]|2[0-8]))?|(\.(\d{1,3}))(?<![a-zA-Z\d])')
+        r'(?<![a-zA-Z\d\.])((([0-9A-Fa-f]{1,4}:){7}([0-9A-Fa-f]{1,4}|:))|(([0-9A-Fa-f]{1,4}:){6}(:[0-9A-Fa-f]{1,4}|((25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)(\.(25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)){3})|:))|(([0-9A-Fa-f]{1,4}:){5}(((:[0-9A-Fa-f]{1,4}){1,2})|:((25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)(\.(25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)){3})|:))|(([0-9A-Fa-f]{1,4}:){4}(((:[0-9A-Fa-f]{1,4}){1,3})|((:[0-9A-Fa-f]{1,4})?:((25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)(\.(25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)){3}))|:))|(([0-9A-Fa-f]{1,4}:){3}(((:[0-9A-Fa-f]{1,4}){1,4})|((:[0-9A-Fa-f]{1,4}){0,2}:((25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)(\.(25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)){3}))|:))|(([0-9A-Fa-f]{1,4}:){2}(((:[0-9A-Fa-f]{1,4}){1,5})|((:[0-9A-Fa-f]{1,4}){0,3}:((25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)(\.(25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)){3}))|:))|(([0-9A-Fa-f]{1,4}:){1}(((:[0-9A-Fa-f]{1,4}){1,6})|((:[0-9A-Fa-f]{1,4}){0,4}:((25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)(\.(25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)){3}))|:))|(:(((:[0-9A-Fa-f]{1,4}){1,7})|((:[0-9A-Fa-f]{1,4}){0,5}:((25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)(\.(25[0-5]|2[0-4]\d|1\d\d|[1-9]?\d)){3}))|:)))(%.+)?(\/[\d][\d]?[\d]?|1([01][0-9]|2[0-8]))?|(\.(\d{1,3}))(?<![a-zA-Z\d])')
 
     potential_ipv6s = re.findall(ipv6_regex, string)
     valid_ipv6s = []
 
     for ipv6 in potential_ipv6s:
         ipv6 = ipv6[0] + ipv6[75]
         if validate_ip(ipv6) is True:
             valid_ipv6s.append(ipv6)
     return netaddr.IPSet(valid_ipv6s)
 
 
-def print_address(address_list, url):
+def print_address(address_set: netaddr.IPSet, url: str) -> None:
     """
     Takes a set of IPv4/IPv6 Addresses as a netaddr.IPSet and prints out
     each address. If no addresses are in the list then an empty address
     warning is printed for the url that was scraped.
-    :param address_list: netaddr.IPSet of addresses to be printed
-    :param url: url that the addresses were scraped from
-    :return: void
     """
-    if address_list:
-        for cidr in address_list.iter_cidrs():
+    if address_set:
+        for cidr in address_set.iter_cidrs():
             print(cidr)
     else:
         print("No addresses found when scraping {}".format(url))
 
 
-def main(url):
+def main(url: str) -> None:
     webpage_text = get_webpage_text(url)
     address_list = ip_from_string(webpage_text)
     addressv6_list = ipv6_from_string(webpage_text)
     print('================\nIPv4 addresses:')
     print_address(address_list, url)
     print('================\nIPv6 addresses:')
     print_address(addressv6_list, url)
 
 
-def entrypoint():
+def entrypoint() -> None:
     url = check_args(sys.argv[1:]).url
     main(url)
 
 
 if __name__ == '__main__':
     entrypoint()
```

### Comparing `ipfromwebpage-1.0.0/pyproject.toml` & `ipfromwebpage-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [tool.poetry]
 name = "ipfromwebpage"
-version = "1.0.0"
+version = "1.1.0"
 description = "Takes a webpage and outputs all ip addresses it finds"
 authors = ["Jay Shepherd <shepherdjay@users.noreply.github.com>"]
 license = "MIT"
 readme = 'README.md'
 repository = 'https://github.com/shepherdjay/ip-from-webpage'
 homepage = 'https://github.com/shepherdjay/ip-from-webpage'
 keywords = ['ipfromwebpage']
 classifiers = [
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.5"
+python = ">=3.7"
 beautifulsoup4 = "^4.4"
-netaddr = "0.7.18"
+netaddr = "^0.8.0"
 
-[tool.poetry.dev-dependencies]
-pytest = "^3.9"
-pytest-cov = "^2.6"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3"
+pytest-cov = "*"
 
 [tool.poetry.scripts]
 ipfromwebpage = 'ipfromwebpage:entrypoint'
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `ipfromwebpage-1.0.0/setup.py` & `ipfromwebpage-1.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 packages = \
 ['ipfromwebpage']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['beautifulsoup4>=4.4,<5.0', 'netaddr==0.7.18']
+['beautifulsoup4>=4.4,<5.0', 'netaddr>=0.8.0,<0.9.0']
 
 entry_points = \
 {'console_scripts': ['ipfromwebpage = ipfromwebpage:entrypoint']}
 
 setup_kwargs = {
     'name': 'ipfromwebpage',
-    'version': '1.0.0',
+    'version': '1.1.0',
     'description': 'Takes a webpage and outputs all ip addresses it finds',
-    'long_description': '## ipfromwebpage\n\n[![PyPi](https://img.shields.io/pypi/v/ipfromwebpage.svg)](https://pypi.python.org/pypi/ipfromwebpage)\n[![Build Status](https://travis-ci.org/shepherdjay/ipfromwebpage.svg?branch=master)](https://travis-ci.org/shepherdjay/ipfromwebpage)\n[![codecov](https://codecov.io/gh/shepherdjay/ipfromwebpage/branch/master/graph/badge.svg)](https://codecov.io/gh/shepherdjay/ipfromwebpage)\n[![Updates](https://pyup.io/repos/github/shepherdjay/ipfromwebpage/shield.svg)](https://pyup.io/repos/github/shepherdjay/ipfromwebpage/)\n\n### Summary:\nTakes a webpage and scrapes for IPv4 Addresses. Then prints the IPs. (aggregated where possible)\n\n#### Quickstart:\n\nInstall using `pip install ipfromwebpage`\n\nRun the code as `ipfromwebpage <url>` where `<url>` is the fully qualified URL you wish to scrap for IPs.\n\n#### Code Example:\n```\nipfromwebpage https://www.cloudflare.com/ips\n================\nIPv4 addresses:\n103.21.244.0/22\n103.22.200.0/22\n103.31.4.0/22\n104.16.0.0/12\n108.162.192.0/18\n131.0.72.0/22\n141.101.64.0/18\n162.158.0.0/15\n172.64.0.0/13\n173.245.48.0/20\n188.114.96.0/20\n190.93.240.0/20\n197.234.240.0/22\n198.41.128.0/17\n================\nIPv6 addresses:\n2400:cb00::/32\n2405:8100::/32\n2405:b500::/32\n2606:4700::/32\n2803:f800::/32\n2a06:98c0::/29\n2c0f:f248::/32\n```\n',
+    'long_description': '## ipfromwebpage\n\n[![PyPi](https://img.shields.io/pypi/v/ipfromwebpage.svg)](https://pypi.python.org/pypi/ipfromwebpage)\n[![CircleCI](https://dl.circleci.com/status-badge/img/gh/shepherdjay/ipfromwebpage/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/shepherdjay/ipfromwebpage/tree/master)\n[![codecov](https://codecov.io/gh/shepherdjay/ipfromwebpage/branch/master/graph/badge.svg)](https://codecov.io/gh/shepherdjay/ipfromwebpage)\n\n### Summary:\nTakes a webpage and scrapes for IPv4 Addresses. Then prints the IPs. (aggregated where possible)\n\n#### Quickstart:\n\nInstall using `pip install ipfromwebpage`\n\nRun the code as `ipfromwebpage <url>` where `<url>` is the fully qualified URL you wish to scrap for IPs.\n\n#### Code Example:\n```\nipfromwebpage https://www.cloudflare.com/ips\n================\nIPv4 addresses:\n103.21.244.0/22\n103.22.200.0/22\n103.31.4.0/22\n104.16.0.0/12\n108.162.192.0/18\n131.0.72.0/22\n141.101.64.0/18\n162.158.0.0/15\n172.64.0.0/13\n173.245.48.0/20\n188.114.96.0/20\n190.93.240.0/20\n197.234.240.0/22\n198.41.128.0/17\n================\nIPv6 addresses:\n2400:cb00::/32\n2405:8100::/32\n2405:b500::/32\n2606:4700::/32\n2803:f800::/32\n2a06:98c0::/29\n2c0f:f248::/32\n```\n',
     'author': 'Jay Shepherd',
     'author_email': 'shepherdjay@users.noreply.github.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/shepherdjay/ip-from-webpage',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.5',
+    'python_requires': '>=3.7',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `ipfromwebpage-1.0.0/PKG-INFO` & `ipfromwebpage-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 Metadata-Version: 2.1
 Name: ipfromwebpage
-Version: 1.0.0
+Version: 1.1.0
 Summary: Takes a webpage and outputs all ip addresses it finds
 Home-page: https://github.com/shepherdjay/ip-from-webpage
 License: MIT
 Keywords: ipfromwebpage
 Author: Jay Shepherd
 Author-email: shepherdjay@users.noreply.github.com
-Requires-Python: >=3.5
-Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.7
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: beautifulsoup4 (>=4.4,<5.0)
-Requires-Dist: netaddr (==0.7.18)
+Requires-Dist: netaddr (>=0.8.0,<0.9.0)
 Project-URL: Repository, https://github.com/shepherdjay/ip-from-webpage
 Description-Content-Type: text/markdown
 
 ## ipfromwebpage
 
 [![PyPi](https://img.shields.io/pypi/v/ipfromwebpage.svg)](https://pypi.python.org/pypi/ipfromwebpage)
-[![Build Status](https://travis-ci.org/shepherdjay/ipfromwebpage.svg?branch=master)](https://travis-ci.org/shepherdjay/ipfromwebpage)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/shepherdjay/ipfromwebpage/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/shepherdjay/ipfromwebpage/tree/master)
 [![codecov](https://codecov.io/gh/shepherdjay/ipfromwebpage/branch/master/graph/badge.svg)](https://codecov.io/gh/shepherdjay/ipfromwebpage)
-[![Updates](https://pyup.io/repos/github/shepherdjay/ipfromwebpage/shield.svg)](https://pyup.io/repos/github/shepherdjay/ipfromwebpage/)
 
 ### Summary:
 Takes a webpage and scrapes for IPv4 Addresses. Then prints the IPs. (aggregated where possible)
 
 #### Quickstart:
 
 Install using `pip install ipfromwebpage`
```


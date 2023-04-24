# Comparing `tmp/pytest_ogsm_plugin-3.5.0.tar.gz` & `tmp/pytest_ogsm_plugin-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_ogsm_plugin-3.5.0.tar", last modified: Mon Apr  3 03:15:54 2023, max compression
+gzip compressed data, was "pytest_ogsm_plugin-3.5.1.tar", last modified: Mon Apr 24 11:11:58 2023, max compression
```

## Comparing `pytest_ogsm_plugin-3.5.0.tar` & `pytest_ogsm_plugin-3.5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-03 03:15:54.860186 pytest_ogsm_plugin-3.5.0/
--rw-r--r--   0 taocw      (501) staff       (20)     1049 2023-04-03 03:15:54.859862 pytest_ogsm_plugin-3.5.0/PKG-INFO
--rw-r--r--   0 taocw      (501) staff       (20)      565 2022-11-15 10:00:14.000000 pytest_ogsm_plugin-3.5.0/README.md
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-03 03:15:54.844516 pytest_ogsm_plugin-3.5.0/gic2api/
--rw-r--r--   0 taocw      (501) staff       (20)       93 2023-02-16 08:41:34.000000 pytest_ogsm_plugin-3.5.0/gic2api/__init__.py
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-03 03:15:54.846156 pytest_ogsm_plugin-3.5.0/gic2api/inpaas/
--rw-r--r--   0 taocw      (501) staff       (20)       93 2023-02-16 08:41:47.000000 pytest_ogsm_plugin-3.5.0/gic2api/inpaas/__init__.py
--rw-r--r--   0 taocw      (501) staff       (20)     1132 2023-02-16 08:42:54.000000 pytest_ogsm_plugin-3.5.0/gic2api/inpaas/test_gic2_lvs.py
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-03 03:15:54.847592 pytest_ogsm_plugin-3.5.0/openapi/
--rw-r--r--   0 taocw      (501) staff       (20)       93 2023-01-09 02:23:24.000000 pytest_ogsm_plugin-3.5.0/openapi/__init__.py
--rw-r--r--   0 taocw      (501) staff       (20)      213 2023-01-09 05:39:17.000000 pytest_ogsm_plugin-3.5.0/openapi/com.py
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-03 03:15:54.849625 pytest_ogsm_plugin-3.5.0/openapi/inpaas/
--rw-r--r--   0 taocw      (501) staff       (20)       93 2023-01-09 02:23:37.000000 pytest_ogsm_plugin-3.5.0/openapi/inpaas/__init__.py
--rw-r--r--   0 taocw      (501) staff       (20)     1453 2023-03-02 06:38:49.000000 pytest_ogsm_plugin-3.5.0/openapi/inpaas/test_haproxy.py
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-03 03:15:54.851595 pytest_ogsm_plugin-3.5.0/pytestOGSMplugin/
--rw-r--r--   0 taocw      (501) staff       (20)       95 2022-11-16 03:20:25.000000 pytest_ogsm_plugin-3.5.0/pytestOGSMplugin/__init__.py
--rw-r--r--   0 taocw      (501) staff       (20)     9715 2023-04-03 03:15:09.000000 pytest_ogsm_plugin-3.5.0/pytestOGSMplugin/pytest_ogsm.py
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-03 03:15:54.853529 pytest_ogsm_plugin-3.5.0/pytestOGSMplugin/templates/
--rw-r--r--   0 taocw      (501) staff       (20)       95 2022-11-16 03:21:06.000000 pytest_ogsm_plugin-3.5.0/pytestOGSMplugin/templates/__init__.py
--rw-r--r--   0 taocw      (501) staff       (20)    28151 2023-03-06 05:38:56.000000 pytest_ogsm_plugin-3.5.0/pytestOGSMplugin/templates/templates.html
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-03 03:15:54.857814 pytest_ogsm_plugin-3.5.0/pytest_ogsm_plugin.egg-info/
--rw-r--r--   0 taocw      (501) staff       (20)     1049 2023-04-03 03:15:54.000000 pytest_ogsm_plugin-3.5.0/pytest_ogsm_plugin.egg-info/PKG-INFO
--rw-r--r--   0 taocw      (501) staff       (20)      622 2023-04-03 03:15:54.000000 pytest_ogsm_plugin-3.5.0/pytest_ogsm_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 taocw      (501) staff       (20)        1 2023-04-03 03:15:54.000000 pytest_ogsm_plugin-3.5.0/pytest_ogsm_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 taocw      (501) staff       (20)       55 2023-04-03 03:15:54.000000 pytest_ogsm_plugin-3.5.0/pytest_ogsm_plugin.egg-info/entry_points.txt
--rw-r--r--   0 taocw      (501) staff       (20)       14 2023-04-03 03:15:54.000000 pytest_ogsm_plugin-3.5.0/pytest_ogsm_plugin.egg-info/requires.txt
--rw-r--r--   0 taocw      (501) staff       (20)       39 2023-04-03 03:15:54.000000 pytest_ogsm_plugin-3.5.0/pytest_ogsm_plugin.egg-info/top_level.txt
--rw-r--r--   0 taocw      (501) staff       (20)       38 2023-04-03 03:15:54.860280 pytest_ogsm_plugin-3.5.0/setup.cfg
--rw-r--r--   0 taocw      (501) staff       (20)     1196 2023-04-03 03:15:31.000000 pytest_ogsm_plugin-3.5.0/setup.py
-drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-03 03:15:54.859000 pytest_ogsm_plugin-3.5.0/tests/
--rw-r--r--   0 taocw      (501) staff       (20)       94 2022-11-15 03:23:31.000000 pytest_ogsm_plugin-3.5.0/tests/__init__.py
--rw-r--r--   0 taocw      (501) staff       (20)      124 2022-11-15 03:23:31.000000 pytest_ogsm_plugin-3.5.0/tests/conftest.py
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.108127 pytest_ogsm_plugin-3.5.1/
+-rw-r--r--   0 taocw      (501) staff       (20)     1049 2023-04-24 11:11:58.107472 pytest_ogsm_plugin-3.5.1/PKG-INFO
+-rw-r--r--   0 taocw      (501) staff       (20)      565 2022-11-15 10:00:14.000000 pytest_ogsm_plugin-3.5.1/README.md
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.081063 pytest_ogsm_plugin-3.5.1/gic2api/
+-rw-r--r--   0 taocw      (501) staff       (20)       93 2023-02-16 08:41:34.000000 pytest_ogsm_plugin-3.5.1/gic2api/__init__.py
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.082712 pytest_ogsm_plugin-3.5.1/gic2api/inpaas/
+-rw-r--r--   0 taocw      (501) staff       (20)       93 2023-02-16 08:41:47.000000 pytest_ogsm_plugin-3.5.1/gic2api/inpaas/__init__.py
+-rw-r--r--   0 taocw      (501) staff       (20)     1132 2023-02-16 08:42:54.000000 pytest_ogsm_plugin-3.5.1/gic2api/inpaas/test_gic2_lvs.py
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.084483 pytest_ogsm_plugin-3.5.1/openapi/
+-rw-r--r--   0 taocw      (501) staff       (20)       93 2023-01-09 02:23:24.000000 pytest_ogsm_plugin-3.5.1/openapi/__init__.py
+-rw-r--r--   0 taocw      (501) staff       (20)      213 2023-01-09 05:39:17.000000 pytest_ogsm_plugin-3.5.1/openapi/com.py
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.086812 pytest_ogsm_plugin-3.5.1/openapi/inpaas/
+-rw-r--r--   0 taocw      (501) staff       (20)       93 2023-01-09 02:23:37.000000 pytest_ogsm_plugin-3.5.1/openapi/inpaas/__init__.py
+-rw-r--r--   0 taocw      (501) staff       (20)     1453 2023-03-02 06:38:49.000000 pytest_ogsm_plugin-3.5.1/openapi/inpaas/test_haproxy.py
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.088855 pytest_ogsm_plugin-3.5.1/pytestOGSMplugin/
+-rw-r--r--   0 taocw      (501) staff       (20)       95 2022-11-16 03:20:25.000000 pytest_ogsm_plugin-3.5.1/pytestOGSMplugin/__init__.py
+-rw-r--r--   0 taocw      (501) staff       (20)    10112 2023-04-24 11:09:11.000000 pytest_ogsm_plugin-3.5.1/pytestOGSMplugin/pytest_ogsm.py
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.093203 pytest_ogsm_plugin-3.5.1/pytestOGSMplugin/templates/
+-rw-r--r--   0 taocw      (501) staff       (20)       95 2022-11-16 03:21:06.000000 pytest_ogsm_plugin-3.5.1/pytestOGSMplugin/templates/__init__.py
+-rw-r--r--   0 taocw      (501) staff       (20)    28151 2023-03-06 05:38:56.000000 pytest_ogsm_plugin-3.5.1/pytestOGSMplugin/templates/templates.html
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.101516 pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/
+-rw-r--r--   0 taocw      (501) staff       (20)     1049 2023-04-24 11:11:58.000000 pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 taocw      (501) staff       (20)      622 2023-04-24 11:11:58.000000 pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 taocw      (501) staff       (20)        1 2023-04-24 11:11:58.000000 pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 taocw      (501) staff       (20)       55 2023-04-24 11:11:58.000000 pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 taocw      (501) staff       (20)       14 2023-04-24 11:11:58.000000 pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/requires.txt
+-rw-r--r--   0 taocw      (501) staff       (20)       39 2023-04-24 11:11:58.000000 pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/top_level.txt
+-rw-r--r--   0 taocw      (501) staff       (20)       38 2023-04-24 11:11:58.108420 pytest_ogsm_plugin-3.5.1/setup.cfg
+-rw-r--r--   0 taocw      (501) staff       (20)     1196 2023-04-24 11:09:38.000000 pytest_ogsm_plugin-3.5.1/setup.py
+drwxr-xr-x   0 taocw      (501) staff       (20)        0 2023-04-24 11:11:58.104357 pytest_ogsm_plugin-3.5.1/tests/
+-rw-r--r--   0 taocw      (501) staff       (20)       94 2022-11-15 03:23:31.000000 pytest_ogsm_plugin-3.5.1/tests/__init__.py
+-rw-r--r--   0 taocw      (501) staff       (20)      124 2022-11-15 03:23:31.000000 pytest_ogsm_plugin-3.5.1/tests/conftest.py
```

### Comparing `pytest_ogsm_plugin-3.5.0/PKG-INFO` & `pytest_ogsm_plugin-3.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_ogsm_plugin
-Version: 3.5.0
+Version: 3.5.1
 Summary: 针对特定项目定制化插件，优化了pytest报告展示方式,并添加了项目所需特定参数
 Home-page: https://github.com/cw010/pytest_ogsm_plugin
 Author: cw
 Author-email: cwalk.t@gmail.com
 License: proprietary
 Keywords: pytest,py.test,pytest_ogsm_plugin
 Platform: UNKNOWN
```

### Comparing `pytest_ogsm_plugin-3.5.0/README.md` & `pytest_ogsm_plugin-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_ogsm_plugin-3.5.0/gic2api/inpaas/test_gic2_lvs.py` & `pytest_ogsm_plugin-3.5.1/gic2api/inpaas/test_gic2_lvs.py`

 * *Files identical despite different names*

### Comparing `pytest_ogsm_plugin-3.5.0/openapi/inpaas/test_haproxy.py` & `pytest_ogsm_plugin-3.5.1/openapi/inpaas/test_haproxy.py`

 * *Files identical despite different names*

### Comparing `pytest_ogsm_plugin-3.5.0/pytestOGSMplugin/pytest_ogsm.py` & `pytest_ogsm_plugin-3.5.1/pytestOGSMplugin/pytest_ogsm.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,60 +147,69 @@
                     })
 
     with open(os.path.join(report_dir, 'history.json'), 'w', encoding='utf-8') as f:
         json.dump(history, f, ensure_ascii=True)
     return history
 
 
+def _is_master(config):
+    """
+    pytest-xdist分布式执行时，判断是主节点master还是子节点
+    主节点没有workerinput属性
+    """
+    return not hasattr(config, 'workerinput')
+
+
 def pytest_sessionfinish(session):
     """在整个测试运行完成之后调用的钩子函数,可以在此处生成测试报告"""
-    report2 = session.config.getoption('--report')
+    if _is_master(session.config):
+        report2 = session.config.getoption('--report')
 
-    if report2:
-        test_result['title'] = session.config.getoption('--title') or '测试报告'
-        test_result['tester'] = session.config.getoption('--tester') or 'QA'
-        test_result['desc'] = session.config.getoption('--desc') or '无'
-        # templates_name = session.config.getoption('--template') or '1'
-        name = report2
-    else:
-        return
-
-    if not name.endswith('.html'):
-        file_name = time.strftime("%Y-%m-%d_%H_%M_%S") + name + '.html'
-    else:
-        file_name = time.strftime("%Y-%m-%d_%H_%M_%S") + name
-
-    if os.path.isdir('reports'):
-        pass
-    else:
-        os.mkdir('reports')
-    file_name = os.path.join('reports', file_name)
-    file_name_index = os.path.join('reports', 'report.html')
-    test_result["run_time"] = '{:.6f} S'.format(time.time() - test_result["start_time"])
-    test_result['all'] = len(test_result['cases'])
-    if test_result['all'] != 0:
-        test_result['pass_rate'] = '{:.2f}'.format(test_result['passed'] / test_result['all'] * 100)
-    else:
-        test_result['pass_rate'] = 0
-    # 保存历史数据
-    test_result['history'] = handle_history_data('reports', test_result)
-    # 渲染报告
-    template_path = os.path.join(os.path.dirname(__file__), './templates')
-    env = Environment(loader=FileSystemLoader(template_path))
-
-    # if templates_name == '1':
-    #     template = env.get_template('templates.html')
-    # else:
-    #     template = env.get_template('templates.html')
-    template = env.get_template('templates.html')
-    report = template.render(test_result)
-    with open(file_name, 'wb') as f:
-        f.write(report.encode('utf8'))
-    with open(file_name_index, 'wb') as f:
-        f.write(report.encode('utf8'))
+        if report2:
+            test_result['title'] = session.config.getoption('--title') or '测试报告'
+            test_result['tester'] = session.config.getoption('--tester') or 'QA'
+            test_result['desc'] = session.config.getoption('--desc') or '无'
+            # templates_name = session.config.getoption('--template') or '1'
+            name = report2
+        else:
+            return
+
+        if not name.endswith('.html'):
+            file_name = time.strftime("%Y-%m-%d_%H_%M_%S") + name + '.html'
+        else:
+            file_name = time.strftime("%Y-%m-%d_%H_%M_%S") + name
+
+        if os.path.isdir('reports'):
+            pass
+        else:
+            os.mkdir('reports')
+        file_name = os.path.join('reports', file_name)
+        file_name_index = os.path.join('reports', 'report.html')
+        test_result["run_time"] = '{:.6f} S'.format(time.time() - test_result["start_time"])
+        test_result['all'] = len(test_result['cases'])
+        if test_result['all'] != 0:
+            test_result['pass_rate'] = '{:.2f}'.format(test_result['passed'] / test_result['all'] * 100)
+        else:
+            test_result['pass_rate'] = 0
+        # 保存历史数据
+        test_result['history'] = handle_history_data('reports', test_result)
+        # 渲染报告
+        template_path = os.path.join(os.path.dirname(__file__), './templates')
+        env = Environment(loader=FileSystemLoader(template_path))
+
+        # if templates_name == '1':
+        #     template = env.get_template('templates.html')
+        # else:
+        #     template = env.get_template('templates.html')
+        template = env.get_template('templates.html')
+        report = template.render(test_result)
+        with open(file_name, 'wb') as f:
+            f.write(report.encode('utf8'))
+        with open(file_name_index, 'wb') as f:
+            f.write(report.encode('utf8'))
 
 
 @pytest.hookimpl(tryfirst=True, hookwrapper=True)
 def pytest_runtest_makereport(item, call):
     outcome = yield
     report = outcome.get_result()
     fixture_extras = getattr(item.config, "extras", [])
```

### Comparing `pytest_ogsm_plugin-3.5.0/pytestOGSMplugin/templates/templates.html` & `pytest_ogsm_plugin-3.5.1/pytestOGSMplugin/templates/templates.html`

 * *Files identical despite different names*

### Comparing `pytest_ogsm_plugin-3.5.0/pytest_ogsm_plugin.egg-info/PKG-INFO` & `pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ogsm-plugin
-Version: 3.5.0
+Version: 3.5.1
 Summary: 针对特定项目定制化插件，优化了pytest报告展示方式,并添加了项目所需特定参数
 Home-page: https://github.com/cw010/pytest_ogsm_plugin
 Author: cw
 Author-email: cwalk.t@gmail.com
 License: proprietary
 Keywords: pytest,py.test,pytest_ogsm_plugin
 Platform: UNKNOWN
```

### Comparing `pytest_ogsm_plugin-3.5.0/pytest_ogsm_plugin.egg-info/SOURCES.txt` & `pytest_ogsm_plugin-3.5.1/pytest_ogsm_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_ogsm_plugin-3.5.0/setup.py` & `pytest_ogsm_plugin-3.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='pytest_ogsm_plugin',
     url='https://github.com/cw010/pytest_ogsm_plugin',
-    version='3.5.0',
+    version='3.5.1',
     author="cw",
     author_email='cwalk.t@gmail.com',
     long_description=read('README.md'),
     long_description_content_type="text/markdown",
     description='针对特定项目定制化插件，优化了pytest报告展示方式,并添加了项目所需特定参数',
     classifiers=[
         'Framework :: Pytest',
```


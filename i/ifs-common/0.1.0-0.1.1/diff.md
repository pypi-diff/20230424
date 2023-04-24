# Comparing `tmp/ifs_common-0.1.0.tar.gz` & `tmp/ifs_common-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifs_common-0.1.0.tar", max compression
+gzip compressed data, was "ifs_common-0.1.1.tar", max compression
```

## Comparing `ifs_common-0.1.0.tar` & `ifs_common-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3295 2023-04-24 02:03:59.058264 ifs_common-0.1.0/README.md
--rw-r--r--   0        0        0      228 2023-04-24 02:13:21.846225 ifs_common-0.1.0/ifsutils/__init__.py
--rw-r--r--   0        0        0     1135 2023-04-24 02:13:21.846762 ifs_common-0.1.0/ifsutils/documentdb_utils.py
--rw-r--r--   0        0        0     2633 2023-04-24 02:13:21.846945 ifs_common-0.1.0/ifsutils/gcs_utils.py
--rw-r--r--   0        0        0     3132 2023-04-24 02:13:21.847108 ifs_common-0.1.0/ifsutils/kafka_utils.py
--rw-r--r--   0        0        0     3043 2023-04-24 02:13:21.847261 ifs_common-0.1.0/ifsutils/postgresql_utils.py
--rw-r--r--   0        0        0     4557 2023-04-24 02:13:21.847433 ifs_common-0.1.0/ifsutils/s3_utils.py
--rw-r--r--   0        0        0      469 2023-04-24 05:35:06.026350 ifs_common-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4143 1970-01-01 00:00:00.000000 ifs_common-0.1.0/setup.py
--rw-r--r--   0        0        0     4045 1970-01-01 00:00:00.000000 ifs_common-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3638 2023-04-24 06:03:27.807765 ifs_common-0.1.1/README.md
+-rw-r--r--   0        0        0      228 2023-04-24 06:35:21.690376 ifs_common-0.1.1/ifsutils/__init__.py
+-rw-r--r--   0        0        0     1604 2023-04-24 06:26:38.848631 ifs_common-0.1.1/ifsutils/documentdb_utils.py
+-rw-r--r--   0        0        0     2323 2023-04-24 06:35:21.699335 ifs_common-0.1.1/ifsutils/gcs_utils.py
+-rw-r--r--   0        0        0     3294 2023-04-24 06:35:21.696815 ifs_common-0.1.1/ifsutils/kafka_utils.py
+-rw-r--r--   0        0        0     3183 2023-04-24 06:35:21.694093 ifs_common-0.1.1/ifsutils/postgresql_utils.py
+-rw-r--r--   0        0        0     5687 2023-04-24 07:06:21.159083 ifs_common-0.1.1/ifsutils/s3_utils.py
+-rw-r--r--   0        0        0      487 2023-04-24 07:10:41.497306 ifs_common-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 ifs_common-0.1.1/setup.py
+-rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 ifs_common-0.1.1/PKG-INFO
```

### Comparing `ifs_common-0.1.0/README.md` & `ifs_common-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # ifs-common
 
-- IFS 코드 작업 시 필요한 utils, library 코드를 모으는 레포지토리이다.
+- IFS 코드 작업 시 필요한 utils, library 코드를 모으는 레포지토리다.
 
 ## 관련 문서
 - Jira: [[UF-1723]](https://42dot.atlassian.net/browse/UF-1723) Util 위치 정리
 
 ## Directory Structure
 
 ```
 ├── README.md
-├── utils
-└── envs
+├── dist  -> pypi 에 패키지 업로드 하기 위해 필요한 파일
+└── ifsutils  -> ifsutils 라는 이름으로 라이브러리(패키지) 등록
+    ├── __init__.py  -> package 시작을 위해 필요
+    ├── documentdb_utils.py
+    ├── gcs_utils.py
+    ├── kafka_utils.py
+    ├── postgresql_utils.py
+    └── s3_utils.py
 ```
 -----
 
 ## Gitflow Guide
 
 ### Branch guide
 - branch 는 main, develop, feature branches, hotfix branches, chore branches 로 구성한다.
```

### Comparing `ifs_common-0.1.0/ifsutils/gcs_utils.py` & `ifs_common-0.1.1/ifsutils/gcs_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,23 @@
 '''
-google service account 를 이용하여 google cloud storage 에 접근하는 함수들을 만들었습니다.
+google service account 를 이용하여 google cloud storage 에 접근하는 함수
 
 API key Google Cloud -> IAM & Admin -> Servie Accounts -> AIoT_rfactor2 -> Key
 cloud storage client : https://cloud.google.com/storage/docs/reference/libraries#client-libraries-install-python
-
 '''
-from google.cloud import storage
 from google import auth
+from google.cloud import storage
 from io import BytesIO
 import pandas as pd
 from time import time
-import os
-import sys
-from dotenv import load_dotenv
-project_dir = os.path.abspath(os.path.dirname('__file__'))
-solution_dir = project_dir.split('library')[0]  # .../ufos-solution 절대 경로
-sys.path.append(solution_dir)
-
-from env_config import absolute_config_reader
-
-GOOGLE_APPLICATION_CREDENTIALS = os.getenv('GOOGLE_APPLICATION_CREDENTIALS')
-# auth.load_credentials_from_file(GOOGLE_APPLICATION_CREDENTIALS)
 
 
-class GoogleCloudStorage():
-    def __init__(self, project_name='UMOS-FII', bucket_name='ufos-solution'):
+class GoogleCloudStorageUtils():
+    def __init__(self, google_application_credential: str = "", project_name: str = 'UMOS-FII', bucket_name: str = 'ufos-solution'):
+        auth.load_credentials_from_file(google_application_credential)
         self.project_name = project_name
         self.bucket_name = bucket_name
         self.client = storage.Client(self.project_name)
         self.bucket = self.client.bucket(self.bucket_name)
 
     def list_blobs_in_condition(self, prefix=None, delimiter=None, should_contain=None, should_delete=None):
         blob_list = [x for x in self.bucket.list_blobs(prefix=prefix, delimiter=delimiter)]
```

### Comparing `ifs_common-0.1.0/ifsutils/kafka_utils.py` & `ifs_common-0.1.1/ifsutils/kafka_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import logging
 import os
 from typing import Callable
-
-from dotenv import load_dotenv
 from kafka import KafkaConsumer, KafkaProducer
 from kafka.errors import KafkaError
 
 logging.basicConfig(format="%(asctime)s %(message)s", datefmt="%Y-%m-%d %I:%M:%S")
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
-load_dotenv(".env")
-load_dotenv("../.env")
-load_dotenv("../../.env")
-
 
-class KafkaProcessor:
-    def __init__(self):
+class KafkaProcessorUtils:
+    def __init__(
+            self,
+            common_bootstrap_servers: str,
+            common_security_protocol: str,
+            common_sasl_mechanism: str,
+            common_sasl_plain_username: str,
+            common_sasl_plain_password: str
+    ):
         self.consumer_group_id = None
-        self.common_bootstrap_servers = os.environ.get("COMMON_BOOTSTRAP_SERVERS")
-        self.common_security_protocol = os.environ.get("COMMON_SECURITY_PROTOCOL")
-        self.common_sasl_mechanism = os.environ.get("COMMON_SASL_MECHANISM")
-        self.common_sasl_plain_username = os.environ.get("COMMON_SASL_PLAIN_USERNAME")
-        self.common_sasl_plain_password = os.environ.get("COMMON_SASL_PLAIN_PASSWORD")
+        self.common_bootstrap_servers = common_bootstrap_servers
+        self.common_security_protocol = common_security_protocol
+        self.common_sasl_mechanism = common_sasl_mechanism
+        self.common_sasl_plain_username = common_sasl_plain_username
+        self.common_sasl_plain_password = common_sasl_plain_password
         self.consumer = None
         self.producer = None
 
-    def get_kafka_consumer(self, consumer_topic: str):
-        self.consumer_group_id = os.environ.get("CONSUMER_GROUP_ID")
+    def get_kafka_consumer(self, consumer_group_id: str, consumer_topic: str):
+        self.consumer_group_id = consumer_group_id
 
         self.consumer = KafkaConsumer(
             consumer_topic,
             group_id=self.consumer_group_id,
             bootstrap_servers=self.common_bootstrap_servers,
             security_protocol=self.common_security_protocol,
             sasl_mechanism=self.common_sasl_mechanism,
@@ -45,38 +46,42 @@
             security_protocol=self.common_security_protocol,
             sasl_mechanism=self.common_sasl_mechanism,
             sasl_plain_username=self.common_sasl_plain_username,
             sasl_plain_password=self.common_sasl_plain_password,
             acks=1,
         )
 
-    def serialize_message_json(self, msg: str, encoder: str = "utf-8"):
+    @staticmethod
+    def _serialize_message_json(msg: str, encoder: str = "utf-8"):
         return msg.encode(encoder)
 
-    def deserialize_message_json(self, msg: bytes, decoder: str = "utf-8"):
+    @staticmethod
+    def _deserialize_message_json(msg: bytes, decoder: str = "utf-8"):
         return msg.decode(decoder)
 
     def run_stream_process(
         self,
+        consumer_group_id: str,
         consumer_topic: str,
         producer_topic: str,
         process_function: Callable[[str], str],
     ):
         self.get_kafka_consumer(
+            consumer_group_id=consumer_group_id,
             consumer_topic=consumer_topic
         )  # os.environ.get("TOPIC_RAW_DATA")
         self.get_kafka_producer()
 
         for message in self.consumer:
             try:
                 # Process the message
-                message_received = self.deserialize_message_json(message.value)
+                message_received = self._deserialize_message_json(message.value)
                 message_to_send = process_function(message_received)
                 logger.info(message_to_send)
                 # Send the processed message to the output topic
                 self.producer.send(
-                    producer_topic, self.serialize_message_json(message_to_send)
+                    producer_topic, self._serialize_message_json(message_to_send)
                 )  # os.environ.get("TOPIC_AGGREGATED_RAW_DATA")
                 self.producer.flush()
 
             except KafkaError as e:
                 logger.error(f"Error while processing message: {str(e)}")
```

### Comparing `ifs_common-0.1.0/ifsutils/postgresql_utils.py` & `ifs_common-0.1.1/ifsutils/postgresql_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import psycopg2
-import os
-import sys
-from dotenv import load_dotenv
-project_dir = os.path.abspath(os.path.dirname('__file__'))
-solution_dir = project_dir.split('library')[0]  # .../ufos-solution 절대 경로
-sys.path.append(solution_dir)
-
-from env_config import absolute_config_reader
-
-HOST = os.getenv("POSTGRESQL_HOST")
-DBNAME = os.getenv("POSTGRESQL_DBNAME")
-USER = os.getenv("POSTGRESQL_USER")
-PW = os.getenv("POSTGRESQL_PW")
-
-
-class PostgreSQL:
-    def __init__(self, host=HOST, dbname=DBNAME, user=USER, pw=PW, port=5432):
-        self.db = psycopg2.connect(
-            host=host,
-            dbname=dbname,
-            user=user,
-            password=pw,
-            port=port
-        )
+import logging
+
+logging.basicConfig(format="%(asctime)s %(message)s", datefmt="%Y-%m-%d %I:%M:%S")
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
+
+
+class PostGreSQLUtils:
+    def __init__(self, host: str, dbname: str, user: str, pw: str, port: str):
+        self.host = host
+        self.dbname = dbname
+        self.user = user
+        self.pw = pw
+        self.port = port
+
+    def _connect_db(self):
+        try:
+            self.db = psycopg2.connect(
+                host=self.host,
+                dbname=self.dbname,
+                user=self.user,
+                password=self.pw,
+                port=self.port
+            )
+        except psycopg2.OperationalError as e:
+            logging.info("E: wrong host number")
+            logging.info(str(e))
+        # TODO: update error type
+
         self.cursor = self.db.cursor()  # allow python code to execute PostgreSQL command in a database session
 
     def __del__(self):
         self.db.close()
         self.cursor.close()
 
     def execute(self, query, **args):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ifs_common-0.1.0/ifsutils/s3_utils.py` & `ifs_common-0.1.1/ifsutils/s3_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,81 @@
 import hashlib
 import hmac
 import logging
-import os
-import socket
-import sys
-import traceback
-import urllib
-from datetime import datetime
 from time import time
-
 import boto3
 from botocore.client import Config
 from botocore.exceptions import ClientError
-from dotenv import load_dotenv
 
-# .../fii-accident-detection 절대 경로
-file_dir = os.path.realpath(__file__)
-project_dir = file_dir.split("s3_libs")[0]
-sys.path.append(project_dir)
-
-logger = logging.getLogger()
-logger.setLevel(logging.INFO)
-formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
-stream_handler = logging.StreamHandler()
-stream_handler.setFormatter(formatter)
-logger.addHandler(stream_handler)
-logger.info(f"file_dir: {file_dir}")
-logger.info(f"project_dir: {project_dir}")
-
-ENV = os.getenv("PHASE")
-logger.info(f"ENV={ENV}")
-load_dotenv(os.path.join(project_dir, f".env.{ENV}"))
-AWS_BUCKET = os.getenv("AWS_BUCKET")
-CDN_URL = os.getenv("CDN_URL")
-logger.info(f"AWS_BUCKET={AWS_BUCKET}")
+logging.basicConfig(format="%(asctime)s %(message)s", datefmt="%Y-%m-%d %I:%M:%S")
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
 
 
 class AmazonWebServiceUtils:
-    def __init__(self, aws_credential_path=None, bucket_name=AWS_BUCKET):
-        """
-        함수를 실행하기 전에 terminal에서 vault-login, vault-auth 를 먼저 진행해줘서 키를 발급해야 된다.
-        자세한 내용은 https://42dot.atlassian.net/wiki/spaces/sec/pages/852197381/AWS 참고
-        """
-        if ENV == "localdev":
-            self.session = boto3.Session(profile_name="common-developer")
-            self.bucket_name = AWS_BUCKET
-            self.aws_credential = self.session.get_credentials()
-
-            logging.debug(f"READ CREDENTIAL FILE :: {self.aws_credential}")
+    def __init__(
+            self,
+            auth_type: str = 'key',
+            bucket_name: str = None,
+            cdn_url: str = None,
+            aws_credential_path: str = None,
+            profile_name: str = 'common-developer'
+    ):
+        self.auth_type = auth_type
+        self.bucket_name = bucket_name
+        self.cdn_url = cdn_url
+        self.aws_credential_path = aws_credential_path  # enter vaulter credential path
+        self.profile_name = profile_name
+
+        if auth_type == 'key':
+            self._init_s3_bucket_with_credential_key()
+        elif auth_type == 'cloud':
+            self._init_s3_bucket_with_resource()
+        else:
+            raise Exception("E: auth_type should be between 'key' and 'cloud'.")
+
+    def _init_s3_bucket_with_resource(self):
+        self.session = boto3.Session(profile_name="common-developer")
+        self.aws_credential = self.session.get_credentials()
+        logging.info("Successfully read aws credential file from cloud")
+        try:
+            self.client = boto3.client("s3", "ap-northeast-2", config=Config(signature_version="s3v4"))
+            self.s3 = boto3.resource("s3", "ap-northeast-2", config=Config(signature_version="s3v4"))
+            self.bucket = self.s3.Bucket(self.bucket_name)
+        except ClientError as e:
+            logging.info("E: S3 client initiating error")
+            logging.info(str(e))
 
-        self.client = boto3.client(
-            "s3", "ap-northeast-2", config=Config(signature_version="s3v4")
-        )
-        self.s3 = boto3.resource(
-            "s3", "ap-northeast-2", config=Config(signature_version="s3v4")
-        )
+    def _init_s3_bucket_with_credential_key(self):
+        self._get_aws_credential_key()
+        try:
+            self.client = boto3.client('s3', **self.aws_credential)
+            self.s3 = boto3.resource('s3', **self.aws_credential)
+            self.bucket = self.s3.Bucket(self.bucket_name)
+        except ClientError as e:
+            logging.info("E: S3 client initiating error")
+            logging.info(str(e))
 
-        self.bucket_name = bucket_name
-        self.bucket = self.s3.Bucket(self.bucket_name)
-        logger.info(self.bucket_name)
+    def _get_aws_credential_key(self):
+        """
+        aws common 계정에 접근하기 위해서는 vaulter로 키를 만들어야 한다.
+        키는 AWS_CREDENTIAL_FILE 위치에 생겨서, 해당 키를 읽고 credential에 접근한다.
+        """
+        self.aws_credential = {}
+        with open(self.aws_credential_path, 'r') as file:
+            for line in file.read().split('\n'):
+                if (line == '') or (line[0] == '['):
+                    continue
+                key, value = line.split(' = ')
+                key = key.strip()
+                value = value.strip()
+                if value[0] == '"':
+                    value = value[1:-1]
+                self.aws_credential.update({key: value})
+        logging.info("Successfully read aws credential file from local")
 
     def s3_list_objects(
         self, prefix="", delimiter="", should_contain=None, should_delete=None
     ):
         paginator = self.client.get_paginator("list_objects_v2")
         pages = paginator.paginate(
             Bucket=self.bucket_name, Prefix=prefix, Delimiter=delimiter
@@ -83,20 +96,20 @@
                 obj
                 for obj in object_list
                 if not any([word in obj["Key"] for word in should_delete])
             ]
         object_name_list = [obj["Key"] for obj in object_list]
         return object_name_list
 
-    def s3_upload_object(self, from_path, key, bucket=""):
+    def s3_upload_file_object(self, from_path, key, bucket=""):
         if not bucket:
             bucket = self.bucket_name
         self.s3.meta.client.upload_file(from_path, bucket, key)
 
-    def s3_upload_objects(self, upload_files, keys, bucket=""):
+    def s3_upload_file_objects(self, upload_files, keys, bucket=""):
         if not bucket:
             bucket = self.bucket_name
         t = time()
         assert len(upload_files) == len(
             keys
         ), "upload_files, keys length should be same"
         length = len(upload_files)
@@ -106,22 +119,28 @@
                 print(f"{i} 번째 uploaded :: {time() - t}")
 
     @staticmethod
     def sign(key, msg):
         return hmac.new(key, msg.encode("utf8"), hashlib.sha256).digest()
 
     def get_signature_key(self, key, date_stamp, region_name, service_name):
-        kDate = self.sign(("AWS4" + key).encode("utf8"), date_stamp)
-        kRegion = self.sign(kDate, region_name)
-        kService = self.sign(kRegion, service_name)
-        kSigning = self.sign(kService, "aws4_request")
-        return kSigning
+        kdate = self.sign(("AWS4" + key).encode("utf8"), date_stamp)
+        kregion = self.sign(kdate, region_name)
+        kservice = self.sign(kregion, service_name)
+        ksigning = self.sign(kservice, "aws4_request")
+        return ksigning
+
+    def s3_upload_memory_object(self, file, to_path, bucket=""):
+        if not bucket:
+            bucket = self.bucket_name
+        object = self.s3.Object(bucket, to_path)
+        object.put(Body=file)
 
-    def create_cdn_url(self, object_key, region="ap-northeast-2", expiration=3600):
-        return CDN_URL + object_key
+    def create_cdn_url(self, object_key):
+        return self.cdn_url + object_key
 
     def get_object(self, key):
         return self.client.get_object(Bucket=self.bucket_name, Key=key)
 
     def download_object(self, from_key, to_path, bucket=""):
         if not bucket:
             bucket = self.bucket_name
```

### Comparing `ifs_common-0.1.0/setup.py` & `ifs_common-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['boto3>=1.26.118,<2.0.0',
  'google-cloud-storage>=2.8.0,<3.0.0',
  'kafka-python>=2.0.2,<3.0.0',
+ 'pandas>=2.0.0,<3.0.0',
  'psycopg-binary>=3.1.8,<4.0.0',
  'psycopg2>=2.9.6,<3.0.0',
  'pymongo>=4.3.3,<5.0.0',
  'python-dotenv>=1.0.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'ifs-common',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
-    'long_description': '# ifs-common\n\n- IFS 코드 작업 시 필요한 utils, library 코드를 모으는 레포지토리이다.\n\n## 관련 문서\n- Jira: [[UF-1723]](https://42dot.atlassian.net/browse/UF-1723) Util 위치 정리\n\n## Directory Structure\n\n```\n├── README.md\n├── utils\n└── envs\n```\n-----\n\n## Gitflow Guide\n\n### Branch guide\n- branch 는 main, develop, feature branches, hotfix branches, chore branches 로 구성한다.\n- feature branch와 지라 이슈는 1:1 연결되도록 생성하며, merge는 develop 브랜치로 한다.\n- branch 이름은 아래의 패턴을 유지한다.\n    - `topic-type/{Jira issue #}-{:desc}`\n        - e.g., `feature/UF-999-test_google_api`\n    - topic types\n        - feature : 기능 추가\n        - hotfix : 버그 수정\n        - chore : 나머지 (리팩토링, 환경변수 설정, 파일 삭제 등)\n- 참고 : [Git branch management](https://42dot.atlassian.net/wiki/spaces/EN/pages/105414823/Git+branch+management)\n\n\n### Commit note guide\n- [Conventional Commit](https://www.conventionalcommits.org/en/v1.0.0/#summary) 을 따른다.\n- commit note 는 아래의 패턴을 유진한다.\n    - `{commit type}: {description}`\n        - e.g., `feat: geolocation mapmatching API added`\n        - commit이 task랑 연결되어 있으면 `feat: [UF-999] desc` 형식으로 적어도 된다.\n    - commit types\n        - `fix`: A bug fix. Correlates with PATCH in SemVer\n        - `feat`: A new feature. Correlates with MINOR in SemVer\n        - `docs`: Documentation only changes\n        - `style`: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-color)\n        - `refactor`: A code change that neither fixes a bug nor adds a feature\n        - `perf`: A code change that improves performance\n        - `test`: Adding missing or correcting existing tests\n        - `build`: Changes that affect the build system or external dependencies (example scopes: pip, docker)\n        - `ci`: Changes to our CI configuration files and scripts (example scopes: GitLabCI)\n- commit 메세지 형식을 유지하기 위해 `commitizen`, `pre-commit` 플러그인을 사용한다.\n    - `fii-accident-reconstruction` 디렉토리의 터미널에서 commit 해야 commitizen 적용 가능\n    - 디렉토리 안에 있는 `.pre-commit-config.yaml` 파일을 기반으로 commit 메세지 형식 검토\n    - 참고 : [Git 환경설정 컨플루언스 문서](https://42dot.atlassian.net/wiki/spaces/UFII/pages/2501869793/WIP+Git)\n\n## Python Guide\n### 가상환경 설정\n- windows 환경에서 실행이 가능하기 때문에 `poetry`를 안쓰고 `python virtualenv`를 사용한다.\n- 가상환경 설정 방법\n  1. 기본 repository 디렉토리에서 `python -m venv {PATH_OF_REPOSITORY}\\venv` 입력\n  2. `.\\venv\\Scripts\\Activate.ps1` 실행\n  3. `python -m pip list`로 가상환경 패키지 확인\n\n### 환경변수 설정\n- 환경변수는 각 프로젝트 별로 하위 디렉토리 밑에 따로 저장한다.\n- 환경변수는 모두 `envs/` 밑에 통합해서 저장한다.\n- 개발환경($ENV, 혹은 $PHASE)에 맞게 .env.$ENV 파일이 생성되어 있다.\n  - `.env.localdev`, .`env.dev`, `.env.int` 등으로 생성\n  - `load_dotenv()` 에서 () 안에 두 환경변수의 경로를 넣어주면 된다.',
+    'long_description': '# ifs-common\n\n- IFS 코드 작업 시 필요한 utils, library 코드를 모으는 레포지토리다.\n\n## 관련 문서\n- Jira: [[UF-1723]](https://42dot.atlassian.net/browse/UF-1723) Util 위치 정리\n\n## Directory Structure\n\n```\n├── README.md\n├── dist  -> pypi 에 패키지 업로드 하기 위해 필요한 파일\n└── ifsutils  -> ifsutils 라는 이름으로 라이브러리(패키지) 등록\n    ├── __init__.py  -> package 시작을 위해 필요\n    ├── documentdb_utils.py\n    ├── gcs_utils.py\n    ├── kafka_utils.py\n    ├── postgresql_utils.py\n    └── s3_utils.py\n```\n-----\n\n## Gitflow Guide\n\n### Branch guide\n- branch 는 main, develop, feature branches, hotfix branches, chore branches 로 구성한다.\n- feature branch와 지라 이슈는 1:1 연결되도록 생성하며, merge는 develop 브랜치로 한다.\n- branch 이름은 아래의 패턴을 유지한다.\n    - `topic-type/{Jira issue #}-{:desc}`\n        - e.g., `feature/UF-999-test_google_api`\n    - topic types\n        - feature : 기능 추가\n        - hotfix : 버그 수정\n        - chore : 나머지 (리팩토링, 환경변수 설정, 파일 삭제 등)\n- 참고 : [Git branch management](https://42dot.atlassian.net/wiki/spaces/EN/pages/105414823/Git+branch+management)\n\n\n### Commit note guide\n- [Conventional Commit](https://www.conventionalcommits.org/en/v1.0.0/#summary) 을 따른다.\n- commit note 는 아래의 패턴을 유진한다.\n    - `{commit type}: {description}`\n        - e.g., `feat: geolocation mapmatching API added`\n        - commit이 task랑 연결되어 있으면 `feat: [UF-999] desc` 형식으로 적어도 된다.\n    - commit types\n        - `fix`: A bug fix. Correlates with PATCH in SemVer\n        - `feat`: A new feature. Correlates with MINOR in SemVer\n        - `docs`: Documentation only changes\n        - `style`: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-color)\n        - `refactor`: A code change that neither fixes a bug nor adds a feature\n        - `perf`: A code change that improves performance\n        - `test`: Adding missing or correcting existing tests\n        - `build`: Changes that affect the build system or external dependencies (example scopes: pip, docker)\n        - `ci`: Changes to our CI configuration files and scripts (example scopes: GitLabCI)\n- commit 메세지 형식을 유지하기 위해 `commitizen`, `pre-commit` 플러그인을 사용한다.\n    - `fii-accident-reconstruction` 디렉토리의 터미널에서 commit 해야 commitizen 적용 가능\n    - 디렉토리 안에 있는 `.pre-commit-config.yaml` 파일을 기반으로 commit 메세지 형식 검토\n    - 참고 : [Git 환경설정 컨플루언스 문서](https://42dot.atlassian.net/wiki/spaces/UFII/pages/2501869793/WIP+Git)\n\n## Python Guide\n### 가상환경 설정\n- windows 환경에서 실행이 가능하기 때문에 `poetry`를 안쓰고 `python virtualenv`를 사용한다.\n- 가상환경 설정 방법\n  1. 기본 repository 디렉토리에서 `python -m venv {PATH_OF_REPOSITORY}\\venv` 입력\n  2. `.\\venv\\Scripts\\Activate.ps1` 실행\n  3. `python -m pip list`로 가상환경 패키지 확인\n\n### 환경변수 설정\n- 환경변수는 각 프로젝트 별로 하위 디렉토리 밑에 따로 저장한다.\n- 환경변수는 모두 `envs/` 밑에 통합해서 저장한다.\n- 개발환경($ENV, 혹은 $PHASE)에 맞게 .env.$ENV 파일이 생성되어 있다.\n  - `.env.localdev`, .`env.dev`, `.env.int` 등으로 생성\n  - `load_dotenv()` 에서 () 안에 두 환경변수의 경로를 넣어주면 된다.',
     'author': 'suhyun.kim',
     'author_email': 'suhyun.kim@42dot.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `ifs_common-0.1.0/PKG-INFO` & `ifs_common-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 Metadata-Version: 2.1
 Name: ifs-common
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: suhyun.kim
 Author-email: suhyun.kim@42dot.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.118,<2.0.0)
 Requires-Dist: google-cloud-storage (>=2.8.0,<3.0.0)
 Requires-Dist: kafka-python (>=2.0.2,<3.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: psycopg-binary (>=3.1.8,<4.0.0)
 Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # ifs-common
 
-- IFS 코드 작업 시 필요한 utils, library 코드를 모으는 레포지토리이다.
+- IFS 코드 작업 시 필요한 utils, library 코드를 모으는 레포지토리다.
 
 ## 관련 문서
 - Jira: [[UF-1723]](https://42dot.atlassian.net/browse/UF-1723) Util 위치 정리
 
 ## Directory Structure
 
 ```
 ├── README.md
-├── utils
-└── envs
+├── dist  -> pypi 에 패키지 업로드 하기 위해 필요한 파일
+└── ifsutils  -> ifsutils 라는 이름으로 라이브러리(패키지) 등록
+    ├── __init__.py  -> package 시작을 위해 필요
+    ├── documentdb_utils.py
+    ├── gcs_utils.py
+    ├── kafka_utils.py
+    ├── postgresql_utils.py
+    └── s3_utils.py
 ```
 -----
 
 ## Gitflow Guide
 
 ### Branch guide
 - branch 는 main, develop, feature branches, hotfix branches, chore branches 로 구성한다.
```


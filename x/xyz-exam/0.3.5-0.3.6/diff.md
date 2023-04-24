# Comparing `tmp/xyz_exam-0.3.5-py3-none-any.whl.zip` & `tmp/xyz_exam-0.3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 30479 bytes, number of entries: 31
+Zip file size: 31480 bytes, number of entries: 32
 -rw-r--r--  2.0 unx       43 b- defN 20-Jan-20 09:10 xyz_exam/__init__.py
 -rw-r--r--  2.0 unx     1631 b- defN 22-Dec-07 08:39 xyz_exam/admin.py
--rw-r--r--  2.0 unx    10615 b- defN 23-Mar-29 09:19 xyz_exam/apis.py
+-rw-r--r--  2.0 unx    12193 b- defN 23-Apr-23 16:47 xyz_exam/apis.py
 -rw-r--r--  2.0 unx      326 b- defN 20-Jan-20 09:08 xyz_exam/apps.py
 -rw-r--r--  2.0 unx     1381 b- defN 22-Oct-27 06:40 xyz_exam/choices.py
 -rw-r--r--  2.0 unx    13585 b- defN 23-Mar-14 03:26 xyz_exam/helper.py
--rw-r--r--  2.0 unx    15318 b- defN 22-Dec-07 08:35 xyz_exam/models.py
+-rw-r--r--  2.0 unx    15556 b- defN 23-Apr-11 14:08 xyz_exam/models.py
 -rw-r--r--  2.0 unx     3688 b- defN 23-Jan-11 04:45 xyz_exam/receivers.py
--rw-r--r--  2.0 unx     3469 b- defN 22-Dec-07 08:35 xyz_exam/serializers.py
+-rw-r--r--  2.0 unx     3469 b- defN 23-Apr-23 16:47 xyz_exam/serializers.py
 -rw-r--r--  2.0 unx     3574 b- defN 22-Jun-23 18:16 xyz_exam/stats.py
 -rw-r--r--  2.0 unx     3154 b- defN 23-Apr-09 13:18 xyz_exam/stores.py
 -rw-r--r--  2.0 unx     7732 b- defN 20-Jan-20 09:14 xyz_exam/migrations/0001_initial.py
 -rw-r--r--  2.0 unx     3123 b- defN 20-Jun-15 13:12 xyz_exam/migrations/0002_auto_20200615_2112.py
 -rw-r--r--  2.0 unx     2514 b- defN 20-Jun-25 21:11 xyz_exam/migrations/0003_auto_20200626_0511.py
 -rw-r--r--  2.0 unx     2405 b- defN 20-Aug-01 16:28 xyz_exam/migrations/0004_auto_20200802_0028.py
 -rw-r--r--  2.0 unx      518 b- defN 20-Sep-01 15:06 xyz_exam/migrations/0005_answer_pictures.py
@@ -21,13 +21,14 @@
 -rw-r--r--  2.0 unx      480 b- defN 21-Jan-06 16:34 xyz_exam/migrations/0009_auto_20210107_0034.py
 -rw-r--r--  2.0 unx     1429 b- defN 21-Mar-31 04:56 xyz_exam/migrations/0010_auto_20210331_1251.py
 -rw-r--r--  2.0 unx     1606 b- defN 22-Sep-08 16:15 xyz_exam/migrations/0011_content.py
 -rw-r--r--  2.0 unx      601 b- defN 22-Sep-17 06:10 xyz_exam/migrations/0012_auto_20220917_1410.py
 -rw-r--r--  2.0 unx      949 b- defN 22-Oct-27 06:41 xyz_exam/migrations/0013_auto_20221027_1441.py
 -rw-r--r--  2.0 unx      498 b- defN 22-Nov-27 11:39 xyz_exam/migrations/0014_paper_parent_id.py
 -rw-r--r--  2.0 unx      484 b- defN 22-Dec-07 08:37 xyz_exam/migrations/0015_paper_is_editable.py
+-rw-r--r--  2.0 unx      946 b- defN 23-Apr-11 14:11 xyz_exam/migrations/0016_auto_20230411_2211.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Jan-20 09:14 xyz_exam/migrations/__init__.py
--rw-r--r--  2.0 unx      987 b- defN 23-Apr-09 15:54 xyz_exam-0.3.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 15:54 xyz_exam-0.3.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-09 15:54 xyz_exam-0.3.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2722 b- defN 23-Apr-09 15:54 xyz_exam-0.3.5.dist-info/RECORD
-31 files, 84483 bytes uncompressed, 26047 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx      987 b- defN 23-Apr-24 16:07 xyz_exam-0.3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 16:07 xyz_exam-0.3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-24 16:07 xyz_exam-0.3.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2824 b- defN 23-Apr-24 16:07 xyz_exam-0.3.6.dist-info/RECORD
+32 files, 87347 bytes uncompressed, 26880 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -72,23 +72,26 @@
 
 Filename: xyz_exam/migrations/0014_paper_parent_id.py
 Comment: 
 
 Filename: xyz_exam/migrations/0015_paper_is_editable.py
 Comment: 
 
+Filename: xyz_exam/migrations/0016_auto_20230411_2211.py
+Comment: 
+
 Filename: xyz_exam/migrations/__init__.py
 Comment: 
 
-Filename: xyz_exam-0.3.5.dist-info/METADATA
+Filename: xyz_exam-0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: xyz_exam-0.3.5.dist-info/WHEEL
+Filename: xyz_exam-0.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: xyz_exam-0.3.5.dist-info/top_level.txt
+Filename: xyz_exam-0.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xyz_exam-0.3.5.dist-info/RECORD
+Filename: xyz_exam-0.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xyz_exam/apis.py

```diff
@@ -208,14 +208,15 @@
         'name': ['exact', 'in'],
         'is_active': ['exact', 'in'],
         'owner_type': ['exact'],
         'owner_id': ['exact', 'in'],
         'begin_time': ['gte', 'lte'],
         'manual_grade': ['exact']
     }
+    ordering_fields = ('minutes', 'question_count', 'begin_time', 'end_time')
 
     @decorators.action(['POST'], detail=False)
     def batch_active(self, request):
         return self.do_batch_action('is_active', True)
 
     @decorators.action(['GET', 'POST'], detail=True)
     def user_answer_signature(self, request, pk):
@@ -260,7 +261,49 @@
     @decorators.action(['GET'], detail=True, permission_classes=[], filter_backends=[])
     def result(self, request, pk):
         error = helper.check_token(request, pk)
         if error:
             return response.Response(error, status=status.HTTP_403_FORBIDDEN)
         exam = self.get_object()
         return response.Response(serializers.ExamResultSerializer(exam).data)
+
+
+    @decorators.action(['POST'], detail=False)
+    def auto_gen(self, request):
+        return super(ExamViewSet, self).create(request)
+
+    def perform_create(self, serializer):
+        super(ExamViewSet, self).perform_create(serializer)
+        if self.action == 'auto_gen':
+            data = self.request.data
+            questions = data.get('questions')
+            exam = serializer.instance
+            from django.contrib.contenttypes.models import ContentType
+            paper, created = models.Paper.objects.update_or_create(
+                owner_id=exam.pk,
+                owner_type=ContentType.objects.get_for_model(exam),
+                defaults=dict(
+                    user=self.request.user,
+                    title=exam.name,
+                    questions_count=len(questions),
+                    tags=exam.tags,
+                    is_editable=False,
+                    is_active=True
+                )
+            )
+            content, created = models.Content.objects.update_or_create(
+                paper=paper,
+                data=dict(
+                    groups=[
+                        {
+                            'title': '选择题',
+                            'number': 1,
+                            'id': 'g0',
+                            'questions': questions
+                        }
+                    ]
+                )
+            )
+            if exam.is_active == False:
+                exam.is_active = True
+                exam.save()
+
```

## xyz_exam/models.py

```diff
@@ -296,14 +296,17 @@
                                         help_text="符合标签的人才能填写问卷,留空则所有人均可填写但不会发个人通知.<p>"
                                                   "例子:<p>老师:张三,李四,赵五<p>学生:*<p>学生.年级:大一,大二<p>学生.入学届别:2019届<p>学生.班级:2018级数字媒体201801班,2018级数字媒体201804班")
     target_user_count = models.PositiveIntegerField('目标参与人数', default=0, blank=True)
     actual_user_count = models.PositiveIntegerField('实际参与人数', default=0, blank=True, null=True)
     target_users = models.ManyToManyField(User, verbose_name='参与人', related_name='exams')
     create_time = models.DateTimeField("创建时间", auto_now_add=True)
     update_time = models.DateTimeField("更新时间", auto_now=True)
+    tags = models.CharField("标记", max_length=64, blank=True, default="")
+    question_filter = modelutils.JSONField("选题条件", default={})
+    question_count = models.PositiveSmallIntegerField('题目数', blank=True, default=0)
     manual_grade = models.BooleanField("人工评分", blank=True, default=False)
     owner_type = models.ForeignKey('contenttypes.ContentType', verbose_name='归类', null=True, blank=True,
                                    on_delete=models.PROTECT)
     owner_id = models.PositiveIntegerField(verbose_name='属主编号', null=True, blank=True, db_index=True)
     owner = GenericForeignKey('owner_type', 'owner_id')
 
     def __str__(self):
```

## Comparing `xyz_exam-0.3.5.dist-info/METADATA` & `xyz_exam-0.3.6.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyz-exam
-Version: 0.3.5
+Version: 0.3.6
 Summary: exam app
 Home-page: https://github.com/szuprefix/py-xyz-exam
 Author: szuprefix
 Author-email: szuprefix@126.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

## Comparing `xyz_exam-0.3.5.dist-info/RECORD` & `xyz_exam-0.3.6.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 xyz_exam/__init__.py,sha256=R09BZ9ss3CC_upX6gf82fFdHuqU_3vh0SavPOcBtQr0,43
 xyz_exam/admin.py,sha256=hP889pXJfcfqy9_5gPq6AYsXE5CyZ8SVYbbR8BjhfQ8,1631
-xyz_exam/apis.py,sha256=qhVu9ocuYmtN3-X8d_se0ha6VaOAGSx11XPZJWEemeg,10615
+xyz_exam/apis.py,sha256=PpuebkLIfnoiYkwIvjRRx-IUlKCPmwJZk_ETDdXz9aI,12193
 xyz_exam/apps.py,sha256=vQwce8vZ81IpBtAVpe8wvqqZXfV0Ht5AJeMY7rRsP6g,326
 xyz_exam/choices.py,sha256=2lKMyQAWnl_yoow98cpQHwqpk-RXxnxij4xcvxeVUko,1381
 xyz_exam/helper.py,sha256=lKVyMH8fOF4JL1wbdr0Hbhm8nFiJWpY2vh3vc_sdvkQ,13585
-xyz_exam/models.py,sha256=EY97WfuQSSl6bhhUihnipfNkbRowjaP3DNluyAedyBI,15318
+xyz_exam/models.py,sha256=gTdNvM6ocVVNEYZRWKzoPs9kFpumRQmnnmxsMe0S1Tw,15556
 xyz_exam/receivers.py,sha256=oOthYcU_vabvgLLAWrjq3BubC7DQbA-ek6_hQhsqhg4,3688
 xyz_exam/serializers.py,sha256=1hNoFpJJwoKBkpxOhrXH7cfw6G-QZO5Dj5C173EUBHU,3469
 xyz_exam/stats.py,sha256=u6XcKw7wkLOm_JtCLoF6241sAZghHQNh5sQfjmjBkSs,3574
 xyz_exam/stores.py,sha256=2T5aMjrMQ4w-qxgkrkx2ZmNcbZq_8lojUZf8dWjGh90,3154
 xyz_exam/migrations/0001_initial.py,sha256=Poa0-alDt7Ylgm6YeJ2cUwNPvHJz55qsuuPTT0IPBR0,7732
 xyz_exam/migrations/0002_auto_20200615_2112.py,sha256=JofSLAwEIoJ1pjZu6MLRiPyWn1nAhxQUuTketVO81Yc,3123
 xyz_exam/migrations/0003_auto_20200626_0511.py,sha256=sAkmKE3fYO9gi9aDOPbZALKZ8T0ZRCvSHiiJjMbRzmM,2514
@@ -20,12 +20,13 @@
 xyz_exam/migrations/0009_auto_20210107_0034.py,sha256=_uvMxxA2V1vwJf_RdrNBVpsXsieOI3so7gU-gkexHGs,480
 xyz_exam/migrations/0010_auto_20210331_1251.py,sha256=terrpUXEcDr0jX_cMWRuM4mLkUUYsSCuragsTs77H4Q,1429
 xyz_exam/migrations/0011_content.py,sha256=FqT4q-o8xJywQ2382G6js1Av7ZEgROr7NmLGSxBp6NU,1606
 xyz_exam/migrations/0012_auto_20220917_1410.py,sha256=RHYolr37Gk2lqZifxypAcylcADeTNZBRRvDGJWAoDmE,601
 xyz_exam/migrations/0013_auto_20221027_1441.py,sha256=_iFsdTKrADPb_EGTTw-3gMD8FMakD8nTbBJOsXRLhY4,949
 xyz_exam/migrations/0014_paper_parent_id.py,sha256=WpMmFmzN2c_4UiSJl2x2QiNv7MZccIbA8kq6M8WWZd8,498
 xyz_exam/migrations/0015_paper_is_editable.py,sha256=8Fbh6vDwxJnKcXar8s6LfGfvAsPdp0vAjxb0XrtjNU0,484
+xyz_exam/migrations/0016_auto_20230411_2211.py,sha256=VuS7lHAoDJ37OpZsBBNKkN-cETJEZ0TJfXxWkKt1-Mk,946
 xyz_exam/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-xyz_exam-0.3.5.dist-info/METADATA,sha256=j7z-fGcg9lNyMZ64K7a18LvtcZQLYUx_vLHWMAHgc8U,987
-xyz_exam-0.3.5.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-xyz_exam-0.3.5.dist-info/top_level.txt,sha256=AdR0uTxGwndkM__gIaBc3_DMomtP0FQ-PKg_WJP2KTE,9
-xyz_exam-0.3.5.dist-info/RECORD,,
+xyz_exam-0.3.6.dist-info/METADATA,sha256=y4Cm2_Vi6n9DY7RZQQ49CQTmEOMp9JHlMdyD5nW3-OA,987
+xyz_exam-0.3.6.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+xyz_exam-0.3.6.dist-info/top_level.txt,sha256=AdR0uTxGwndkM__gIaBc3_DMomtP0FQ-PKg_WJP2KTE,9
+xyz_exam-0.3.6.dist-info/RECORD,,
```


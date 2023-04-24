# Comparing `tmp/xyz_course-0.1.2-py3-none-any.whl.zip` & `tmp/xyz_course-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 9039 bytes, number of entries: 17
+Zip file size: 9175 bytes, number of entries: 17
 -rw-r--r--  2.0 unx       45 b- defN 20-Jan-22 15:29 xyz_course/__init__.py
 -rw-r--r--  2.0 unx      735 b- defN 20-Oct-25 04:09 xyz_course/admin.py
--rw-r--r--  2.0 unx     2506 b- defN 21-Jun-05 23:14 xyz_course/apis.py
+-rw-r--r--  2.0 unx     2724 b- defN 23-Mar-06 17:25 xyz_course/apis.py
 -rw-r--r--  2.0 unx      332 b- defN 20-Jan-22 15:33 xyz_course/apps.py
--rw-r--r--  2.0 unx     3395 b- defN 22-Sep-25 01:15 xyz_course/models.py
--rw-r--r--  2.0 unx     1470 b- defN 22-Oct-22 15:18 xyz_course/serializers.py
+-rw-r--r--  2.0 unx     3539 b- defN 23-Mar-06 17:18 xyz_course/models.py
+-rw-r--r--  2.0 unx     1684 b- defN 23-Apr-13 16:14 xyz_course/serializers.py
 -rw-r--r--  2.0 unx      662 b- defN 20-Dec-24 16:59 xyz_course/stats.py
 -rw-r--r--  2.0 unx     3903 b- defN 20-Jan-23 10:17 xyz_course/migrations/0001_initial.py
 -rw-r--r--  2.0 unx      676 b- defN 20-Jun-15 08:23 xyz_course/migrations/0002_auto_20200615_1623.py
 -rw-r--r--  2.0 unx      697 b- defN 20-Jun-15 11:13 xyz_course/migrations/0003_auto_20200615_1913.py
 -rw-r--r--  2.0 unx     1704 b- defN 20-Oct-25 01:10 xyz_course/migrations/0004_auto_20201025_0910.py
 -rw-r--r--  2.0 unx      516 b- defN 21-Jun-01 15:58 xyz_course/migrations/0005_course_data.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Jan-23 10:17 xyz_course/migrations/__init__.py
--rw-r--r--  2.0 unx      955 b- defN 22-Oct-27 07:28 xyz_course-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Oct-27 07:28 xyz_course-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 22-Oct-27 07:28 xyz_course-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1435 b- defN 22-Oct-27 07:28 xyz_course-0.1.2.dist-info/RECORD
-17 files, 19134 bytes uncompressed, 6653 bytes compressed:  65.2%
+-rw-r--r--  2.0 unx      955 b- defN 23-Apr-24 18:19 xyz_course-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 18:19 xyz_course-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-24 18:19 xyz_course-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1435 b- defN 23-Apr-24 18:19 xyz_course-0.1.3.dist-info/RECORD
+17 files, 19710 bytes uncompressed, 6789 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: xyz_course/migrations/0005_course_data.py
 Comment: 
 
 Filename: xyz_course/migrations/__init__.py
 Comment: 
 
-Filename: xyz_course-0.1.2.dist-info/METADATA
+Filename: xyz_course-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xyz_course-0.1.2.dist-info/WHEEL
+Filename: xyz_course-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xyz_course-0.1.2.dist-info/top_level.txt
+Filename: xyz_course-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xyz_course-0.1.2.dist-info/RECORD
+Filename: xyz_course-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xyz_course/apis.py

```diff
@@ -33,14 +33,18 @@
             user=request.user,
             defaults=dict(
                 is_pass=request.data.get('is_pass')
             )
         )
         return response.Response(dict(detail='ok'))
 
+    def get_serializer_class(self):
+        if self.request.query_params.get('get_outline_list'):
+            return serializers.CourseOutlineSerializer
+        return super(CourseViewSet, self).get_serializer_class()
 
 @register()
 class CategoryViewSet(viewsets.ModelViewSet):
     queryset = models.Category.objects.all()
     serializer_class = serializers.CategorySerializer
     search_fields = ('name', 'code')
     filter_fields = ('code', 'name')
```

## xyz_course/models.py

```diff
@@ -41,14 +41,21 @@
             yield c
 
     @cached_property
     def outline_treenode(self):
         from xyz_util.textutils import hierarchy
         return hierarchy(self.outline, ['第(\d+)章','\n+\s*(\d+)\.'])
 
+    @cached_property
+    def outline_list(self):
+        rs = []
+        for a in list(self):
+            rs += a.to_array()
+        return rs
+
     def save(self, **kwargs):
         if self.is_active is None:
             self.is_active = True
         super(Course, self).save(**kwargs)
 
 
 class Chapter(CodeMixin, models.Model):
```

## xyz_course/serializers.py

```diff
@@ -23,14 +23,22 @@
 
 class CourseNameSerializer(serializers.ModelSerializer):
     class Meta:
         model = models.Course
         fields = ('name',)
 
 
+class CourseOutlineSerializer(serializers.ModelSerializer):
+    outline_list = serializers.ListField(read_only=True)
+    class Meta:
+        model = models.Course
+        fields = ('id', 'name', 'outline_list')
+
+
+
 class CategorySerializer(IDAndStrFieldSerializerMixin, serializers.ModelSerializer):
     class Meta:
         model = models.Category
         fields = '__all__'
 
 
 class ChapterSerializer(IDAndStrFieldSerializerMixin, serializers.ModelSerializer):
```

## Comparing `xyz_course-0.1.2.dist-info/METADATA` & `xyz_course-0.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyz-course
-Version: 0.1.2
+Version: 0.1.3
 Summary: course
 Home-page: https://github.com/szuprefix/py-xyz-course
 Author: szuprefix
 Author-email: szuprefix@126.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

## Comparing `xyz_course-0.1.2.dist-info/RECORD` & `xyz_course-0.1.3.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 xyz_course/__init__.py,sha256=HmprY0CSLD8J0QbbpCgj2vrVewCij5Il2ntztTBgjtA,45
 xyz_course/admin.py,sha256=khPx1G49iFJkfRa1PgEoeCaIk3MwZLl1ugRiVOIYRhE,735
-xyz_course/apis.py,sha256=DYzNO3ZE1wSrDpGihh5TTzN1iy1qW8bGm0Tyn4jfw5s,2506
+xyz_course/apis.py,sha256=Fkc4eRcOcShJ0tABtIFboPNcf4ReFcUK2d3gyENl6oU,2724
 xyz_course/apps.py,sha256=4uWoLj5NwCU5Sdr9q_2Anc94hqntIjDRIekVxvj2-zg,332
-xyz_course/models.py,sha256=y15-JBRi_nNEgT6EsnZx_FE6gUwx8_U6iC65X9gtAFY,3395
-xyz_course/serializers.py,sha256=4cFiQ3Ii1KcyCu3gFVM5JjHlvv3vkxIUPWQit8FykvU,1470
+xyz_course/models.py,sha256=h32Lsi4vHEw3EOXKO8nGsNOooOefTNXTSLbumxZ0vIE,3539
+xyz_course/serializers.py,sha256=PsHoQX-E2-P_65TVinlK_l8gGwOOAwjMMfEioyW32Rc,1684
 xyz_course/stats.py,sha256=u7BruKsBYKRV1CwNE6zki52p944uPx-yhXdxiJN33-w,662
 xyz_course/migrations/0001_initial.py,sha256=n7M4X4ED5EYoNlYklbivKg2nOtYUAjZoYO_sUu5AVBI,3903
 xyz_course/migrations/0002_auto_20200615_1623.py,sha256=3ZhBK_kc411GysYabjnKN4iMOyCI_heDe4y1lECh64k,676
 xyz_course/migrations/0003_auto_20200615_1913.py,sha256=_tGZv68o1WmxWKBPMUNhyQqLLfKWY-UEWOgl3iaNZBY,697
 xyz_course/migrations/0004_auto_20201025_0910.py,sha256=ZEYR9BBqCL9sk3XKXD3YNH6DWUFSmymg8_zNY11oD24,1704
 xyz_course/migrations/0005_course_data.py,sha256=5_sTc2Thc8MQtjPM-7vQSdUfCAOb_xq_nw4dRKXGEkM,516
 xyz_course/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-xyz_course-0.1.2.dist-info/METADATA,sha256=YEFnoregCnnlAd6hGXDseHWE3YkNnjbJ0xvsjgBdhgQ,955
-xyz_course-0.1.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-xyz_course-0.1.2.dist-info/top_level.txt,sha256=tjrDjC_voBSaxk-aogj477tvuafksqYaVLxHtuCR6qk,11
-xyz_course-0.1.2.dist-info/RECORD,,
+xyz_course-0.1.3.dist-info/METADATA,sha256=RJNHovB26C7H6QDcI1i-KSkmC4ttw4-RIYMkt6VNI6w,955
+xyz_course-0.1.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+xyz_course-0.1.3.dist-info/top_level.txt,sha256=tjrDjC_voBSaxk-aogj477tvuafksqYaVLxHtuCR6qk,11
+xyz_course-0.1.3.dist-info/RECORD,,
```


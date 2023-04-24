# Comparing `tmp/pystructs3-0.0.2.tar.gz` & `tmp/pystructs3-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystructs3-0.0.2.tar", last modified: Tue Apr 18 21:32:43 2023, max compression
+gzip compressed data, was "pystructs3-0.0.3.tar", last modified: Mon Apr 24 00:11:15 2023, max compression
```

## Comparing `pystructs3-0.0.2.tar` & `pystructs3-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:32:43.243517 pystructs3-0.0.2/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-04-18 21:12:24.000000 pystructs3-0.0.2/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-04-18 21:32:43.243517 pystructs3-0.0.2/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      798 2023-04-18 21:13:45.000000 pystructs3-0.0.2/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:32:43.239517 pystructs3-0.0.2/pystructs/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      559 2023-04-18 07:09:08.000000 pystructs3-0.0.2/pystructs/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     7711 2023-04-18 21:28:14.000000 pystructs3-0.0.2/pystructs/base.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1792 2023-04-18 21:30:34.000000 pystructs3-0.0.2/pystructs/codec.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:32:43.239517 pystructs3-0.0.2/pystructs/struct/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      310 2023-04-18 07:09:01.000000 pystructs3-0.0.2/pystructs/struct/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3020 2023-04-18 21:30:44.000000 pystructs3-0.0.2/pystructs/struct/fields.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     4806 2023-04-18 20:53:05.000000 pystructs3-0.0.2/pystructs/struct/struct.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:32:43.243517 pystructs3-0.0.2/pystructs3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-04-18 21:32:43.000000 pystructs3-0.0.2/pystructs3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      337 2023-04-18 21:32:43.000000 pystructs3-0.0.2/pystructs3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-04-18 21:32:43.000000 pystructs3-0.0.2/pystructs3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       30 2023-04-18 21:32:43.000000 pystructs3-0.0.2/pystructs3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       10 2023-04-18 21:32:43.000000 pystructs3-0.0.2/pystructs3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-04-18 21:32:43.243517 pystructs3-0.0.2/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      763 2023-04-18 21:32:25.000000 pystructs3-0.0.2/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-24 00:11:15.760621 pystructs3-0.0.3/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-04-18 21:12:24.000000 pystructs3-0.0.3/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-04-24 00:11:15.760621 pystructs3-0.0.3/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      798 2023-04-18 21:13:45.000000 pystructs3-0.0.3/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-24 00:11:15.760621 pystructs3-0.0.3/pystructs/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      681 2023-04-21 06:27:06.000000 pystructs3-0.0.3/pystructs/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     8814 2023-04-23 23:27:43.000000 pystructs3-0.0.3/pystructs/base.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1928 2023-04-19 00:40:15.000000 pystructs3-0.0.3/pystructs/codec.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2798 2023-04-21 06:25:07.000000 pystructs3-0.0.3/pystructs/list.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-24 00:11:15.760621 pystructs3-0.0.3/pystructs/struct/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      332 2023-04-19 00:33:47.000000 pystructs3-0.0.3/pystructs/struct/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     3097 2023-04-19 00:21:42.000000 pystructs3-0.0.3/pystructs/struct/fields.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     5133 2023-04-21 07:24:30.000000 pystructs3-0.0.3/pystructs/struct/struct.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-24 00:11:15.760621 pystructs3-0.0.3/pystructs3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-04-24 00:11:15.000000 pystructs3-0.0.3/pystructs3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      355 2023-04-24 00:11:15.000000 pystructs3-0.0.3/pystructs3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-04-24 00:11:15.000000 pystructs3-0.0.3/pystructs3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       30 2023-04-24 00:11:15.000000 pystructs3-0.0.3/pystructs3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       10 2023-04-24 00:11:15.000000 pystructs3-0.0.3/pystructs3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-04-24 00:11:15.760621 pystructs3-0.0.3/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      763 2023-04-24 00:10:56.000000 pystructs3-0.0.3/setup.py
```

### Comparing `pystructs3-0.0.2/LICENSE` & `pystructs3-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.2/PKG-INFO` & `pystructs3-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystructs3
-Version: 0.0.2
+Version: 0.0.3
 Summary: Dataclass-Like Serialization Helpers for More Complex Data-Types
 Home-page: https://github.com/imgurbot12/pystruct
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pystructs3-0.0.2/README.md` & `pystructs3-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.2/pystructs/__init__.py` & `pystructs3-0.0.3/pystructs/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Python Struct Utilities Library
 """
+from .list import *
 from .base import *
 from .codec import *
 
 #** Variables **#
 __all__ = [
     'Codec',
     'Context',
@@ -17,20 +18,26 @@
     'Int64',
     'IpAddr',
     'Ipv4',
     'Ipv6',
     'MacAddr',
     'SizedBytes',
     'StaticBytes',
+    'GreedyBytes',
     'Domain',
+    'SizedList',
+    'StaticList',
+    'GreedyList',
 
     'field',
+    'fields',
     'struct',
     'make_struct',
     'Struct',
+    'Property',
 ]
 
 Int8  = Int[8]
 Int16 = Int[16]
 Int32 = Int[32]
 Int48 = Int[48]
 Int64 = Int[64]
```

### Comparing `pystructs3-0.0.2/pystructs/base.py` & `pystructs3-0.0.3/pystructs/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 Base Common Sequence Types
 """
+from abc import abstractmethod
 import re
 from ipaddress import IPv4Address, IPv6Address
-from typing import ClassVar, Callable, Any, Union, Type
+from typing import ClassVar, Callable, Any, Protocol, Union, Type
+from typing_extensions import runtime_checkable
 
 from .codec import Codec, Context
 
 #** Variables **#
 __all__ = [
     'Const',
     'Int',
     'IpAddr',
     'MacAddr',
     'SizedBytes',
     'StaticBytes',
+    'GreedyBytes',
     'Domain',
 ]
 
 #** Functions **#
 
 def codec(name: str, base: Type[Codec], **kwargs) -> Type[Codec]:
     """spawn new singleton codec type"""
@@ -36,27 +39,38 @@
     base_type: type
 
     def __class_getitem__(cls, const: bytes) -> Type[Codec]:
         """generate const type w/ given const"""
         name = cls.__name__
         return codec(f'{name}[{const!r}]', cls, 
             size=len(const), default=const, base_type=bytes)
+    
+    @classmethod
+    def sizeof(cls) -> int:
+        return cls.size
 
     @classmethod
     def encode(cls, ctx: Context, value: bytes) -> bytes:
         assert value == cls.default, f'{value} does not match {cls}'
         ctx.index += cls.size
         return cls.default
     
     @classmethod
     def decode(cls, ctx: Context, raw: bytes) -> bytes:
         value = ctx.slice(raw, cls.size)
         assert value == cls.default, f'{value} does not match {cls}'
         return value
 
+@runtime_checkable
+class IntLike(Protocol):
+
+    @abstractmethod
+    def __int__(self) -> int:
+        raise NotImplementedError
+
 class Int(Codec):
     """
     Variable Size Integer Codec Definition
 
     Examples: Int[16], Int[32], Int[64, MyIntEnum]
     """
     size: ClassVar[int]
@@ -66,20 +80,24 @@
     def __class_getitem__(cls, s: Union[int, tuple]) -> Type[Codec]:
         """generate custom Int subclass with the given options"""
         size = s if isinstance(s, int) else s[0]
         wrap = s[1] if isinstance(s, tuple) and len(s) > 1 else lambda x: x
         name = s[2] if isinstance(s, tuple) and len(s) > 2 else cls.__name__
         assert size % 8 == 0, 'size must be multiple of eight'
         cname = f'{name}[{size}]'
-        return codec(cname, cls, size=size // 8, wrap=wrap, base_type=int)
+        return codec(cname, cls, size=size // 8, wrap=wrap, base_type=IntLike)
+    
+    @classmethod
+    def sizeof(cls) -> int:
+        return cls.size
 
     @classmethod
-    def encode(cls, ctx: Context, value: int) -> bytes:
+    def encode(cls, ctx: Context, value: IntLike) -> bytes:
         ctx.index += cls.size
-        return value.to_bytes(cls.size, 'big')
+        return int(value).to_bytes(cls.size, 'big')
 
     @classmethod
     def decode(cls, ctx: Context, raw: bytes) -> int:
         data = ctx.slice(raw, cls.size)
         size = cls.size * 8
         assert len(data) == cls.size, f'len(bytes)[{len(data)}] != Int[{size}]'
         value = int.from_bytes(data, 'big')
@@ -89,27 +107,32 @@
     """
     Ipv4/Ipv6 Address Variable Codec Definition
 
     Example: IpAddr['ipv4'] or IpAddr['ipv6']
     """
     size:      int
     ip_type:   Union[Type[IPv4Address], Type[IPv6Address]]
-    base_type: Union[type, tuple] = (str, bytes)
+    base_type: Union[type, tuple] = (str, bytes, IPv4Address)
 
     def __class_getitem__(cls, iptype: str) -> Type[Codec]:
         """generate ipv4 or ipv6 ipaddress supporting codec type"""
         assert iptype in ('ipv4', 'ipv6'), 'invalid ipaddress type'
         size = 4 if iptype == 'ipv4' else 16
         addr = IPv4Address if iptype == 'ipv4' else IPv6Address
         return codec(f'IPv{iptype[-1]}', cls, size=size, ip_type=addr)
 
     @classmethod
+    def sizeof(cls) -> int:
+        return cls.size
+
+    @classmethod
     def encode(cls, ctx: Context, value: Union[str, bytes]) -> bytes:
-        packed = cls.ip_type(value).packed
-        ctx.index += len(packed)
+        ipaddr = value if isinstance(value, cls.ip_type) else cls.ip_type(value)
+        packed = ipaddr.packed
+        ctx.index += cls.size
         return packed
 
     @classmethod
     def decode(cls, ctx: Context, raw: bytes) -> Union[IPv4Address, IPv6Address]:
         data = ctx.slice(raw, cls.size)
         return cls.ip_type(data)
 
@@ -117,14 +140,18 @@
     """
     Serialized MacAddress Codec
     """
     base_type: type       = str
     replace:   re.Pattern = re.compile('[:.-]')
   
     @classmethod
+    def sizeof(cls) -> int:
+        return 6
+
+    @classmethod
     def encode(cls, ctx: Context, value: str) -> bytes:
         content = bytes.fromhex(cls.replace.sub('', value))
         ctx.index += len(content)
         return content
 
     @classmethod
     def decode(cls, ctx: Context, raw: bytes) -> str:
@@ -132,15 +159,15 @@
 
 class SizedBytes(Codec):
     """
     Variable Sized Bytes Codec with Length Denoted by Prefixed Integer
 
     Example: SizedBytes[32]
     """
-    hint:      Codec
+    hint:      Int
     base_type: type
  
     def __class_getitem__(cls, hint: int) -> Type[Codec]:
         name   = cls.__name__
         hcodec = Int[hint]
         return codec(f'{name}[{hint!r}]', cls, hint=hcodec, base_type=bytes)
 
@@ -163,26 +190,47 @@
     """
     size:      int
     base_type: type
 
     def __class_getitem__(cls, size: int) -> Type[Codec]:
         name = cls.__name__
         return codec(f'{name}[{size!r}]', cls, size=size, base_type=bytes)
+    
+    @classmethod
+    def sizeof(cls) -> int:
+        return cls.size
 
     @classmethod
     def encode(cls, ctx: Context, content: bytes) -> bytes:
         assert len(content) <= cls.size, f'len(content) >= {cls.size} bytes'
         ctx.index += cls.size
         content = content.ljust(cls.size, b'\x00')
         return content
 
     @classmethod
     def decode(cls, ctx: Context, raw: bytes) -> bytes:
         return ctx.slice(raw, cls.size).rstrip(b'\x00')
 
+class GreedyBytes(Codec):
+    """
+    Variable Bytes that Greedily Collects all Bytes left in Data
+    """
+    base_type: type = bytes
+ 
+    @classmethod
+    def encode(cls, ctx: Context, value: Any) -> bytes:
+        ctx.index += len(value)
+        return value
+
+    @classmethod
+    def decode(cls, ctx: Context, raw: bytes) -> bytes:
+        data = raw[ctx.index:]
+        ctx.index += len(data)
+        return data
+
 class Domain(Codec):
     """
     DNS Style Domain Serialization w/ Index Pointers to Eliminate Duplicates
     """
     ptr_mask:  int  = 0xC0
     base_type: type = bytes
```

### Comparing `pystructs3-0.0.2/pystructs/codec.py` & `pystructs3-0.0.3/pystructs/codec.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,19 @@
 
 @runtime_checkable
 class Codec(Protocol):
     """Encoding/Decoding Codec Protocol"""
     init:      ClassVar[bool] = True
     default:   ClassVar[Any]  = None
     base_type: type
+    
+    @classmethod
+    def sizeof(cls) -> int:
+        name = cls.__name__
+        raise RuntimeError(f'Cannot get sizeof {name!r}')
 
     @classmethod
     @abstractmethod
     def encode(cls, ctx: Context, value: Any) -> bytes:
         raise NotImplementedError
 
     @classmethod
```

### Comparing `pystructs3-0.0.2/pystructs/struct/fields.py` & `pystructs3-0.0.3/pystructs/struct/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,17 @@
     # raise error on unsupported type
     raise ValueError(f'invalid annotatation: {name!r}: {anno}')
 
 #** Classes **#
 
 @dataclass
 class Property:
-    hint: type
+    hint:    type
+    init:    ClassVar[bool] = False
+    default: ClassVar[Any]  = MISSING
 
     def __class_getitem__(cls, hint: type) -> Self:
         return cls(hint)
 
 @dataclass
 class Field:
     name:     str
```

### Comparing `pystructs3-0.0.2/pystructs/struct/struct.py` & `pystructs3-0.0.3/pystructs/struct/struct.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,33 @@
 from typing import Optional, Dict, Type, Generic, TypeVar
 from typing_extensions import Self, dataclass_transform
 
 from .fields import *
 from ..base import Context, Codec
 
 #** Variables **#
-__all__ = ['struct', 'make_struct', 'Struct']
+__all__ = ['fields', 'struct', 'make_struct', 'Struct']
 
 #: generic typevar to help with type definitions
 T = TypeVar('T')
 
 #: codec-fields field on class objects
 FIELDS = '__encoded__'
 
 #: annotations field on class objects
 ANNOTATIONS = '__annotations__'
 
 #** Functions **#
 
+def fields(struct) -> Dict[str, Field]:
+    """
+    retrieve list of fields associated w/ the specified struct
+    """
+    return getattr(struct, FIELDS)
+
 def struct(cls: Optional[Type[T]] = None, **kwargs) -> Type['Struct[T]']:
     """
     generate sequence object w/ codec-field and build dataclass-like object
 
     :param cls:    class object being converted into a sequence
     :param kwargs: kwargs to pass to dataclass generation
     :return:       sequence class object type
@@ -49,14 +55,16 @@
     values      = {}
     fields      = getattr(cls, FIELDS, OrderedDict())
     annotations = getattr(cls, ANNOTATIONS, {})
     for name in list(annotations.keys()):
         # skip processing if annotation is a InitVar or ClassVar
         anno = annotations[name]
         if is_datavar(anno):
+            if name in fields:
+                del fields[name]
             continue
         # retrieve default value
         value = getattr(cls, name, MISSING)
         if hasattr(cls, name):
             delattr(cls, name)
         # parse attribute into field if not already
         anno  = compile_annotation(name, anno)
@@ -65,14 +73,15 @@
         fields[name] = field
         # process property types
         if isinstance(anno, Property):
             # ensure annotation is deleted for dataclass
             del annotations[name]
             field.type     = anno.hint
             field.dataattr = False
+            value          = value.default
             # validate property function value
             if not isinstance(value, property):
                 if not callable(value):
                     raise ValueError(f'property: {name} must be a function')
                 value = property(value)
             values[name] = value
             continue
@@ -82,14 +91,16 @@
             field.default     = anno.default or field.default
             annotations[name] = anno.base_type
             values[name]      = value
     # generate bases for new sequence dataclass
     bases = list(cls.__mro__)
     if Struct not in bases:
         bases.insert(1, Struct)
+    if Generic in bases:
+        bases.remove(Generic)
     # generate new unique object w/ fields parsed from original
     dataclassfunc = dataclasses.dataclass(**kwargs)
     return dataclassfunc(type(cname(cls), tuple(bases), { #type: ignore
         FIELDS:      fields,
         ANNOTATIONS: annotations,
         **{k:v for k,v in values.items() if v is not MISSING}
     }))
```

### Comparing `pystructs3-0.0.2/pystructs3.egg-info/PKG-INFO` & `pystructs3-0.0.3/pystructs3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystructs3
-Version: 0.0.2
+Version: 0.0.3
 Summary: Dataclass-Like Serialization Helpers for More Complex Data-Types
 Home-page: https://github.com/imgurbot12/pystruct
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pystructs3-0.0.2/setup.py` & `pystructs3-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name='pystructs3',
-    version='0.0.2',
+    version='0.0.3',
     license='MIT',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     url='https://github.com/imgurbot12/pystruct',
     description="Dataclass-Like Serialization Helpers for More Complex Data-Types",
     long_description=readme,
     long_description_content_type="text/markdown",
```


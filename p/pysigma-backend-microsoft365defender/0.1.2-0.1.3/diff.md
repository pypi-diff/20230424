# Comparing `tmp/pysigma_backend_microsoft365defender-0.1.2.tar.gz` & `tmp/pysigma_backend_microsoft365defender-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_microsoft365defender-0.1.2.tar", max compression
+gzip compressed data, was "pysigma_backend_microsoft365defender-0.1.3.tar", max compression
```

## Comparing `pysigma_backend_microsoft365defender-0.1.2.tar` & `pysigma_backend_microsoft365defender-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7653 2023-04-17 22:32:30.277807 pysigma_backend_microsoft365defender-0.1.2/LICENSE
--rw-r--r--   0        0        0      626 2023-04-17 22:32:30.277807 pysigma_backend_microsoft365defender-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      407 2023-04-17 22:32:30.277807 pysigma_backend_microsoft365defender-0.1.2/sigma/backends/microsoft365defender/__init__.py
--rw-r--r--   0        0        0    11533 2023-04-17 22:32:30.277807 pysigma_backend_microsoft365defender-0.1.2/sigma/backends/microsoft365defender/microsoft365defender.py
--rw-r--r--   0        0        0      315 2023-04-17 22:32:30.277807 pysigma_backend_microsoft365defender-0.1.2/sigma/pipelines/microsoft365defender/__init__.py
--rw-r--r--   0        0        0    29236 2023-04-17 22:32:30.277807 pysigma_backend_microsoft365defender-0.1.2/sigma/pipelines/microsoft365defender/microsoft365defender.py
--rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 pysigma_backend_microsoft365defender-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     7653 2023-04-24 17:56:47.544492 pysigma_backend_microsoft365defender-0.1.3/LICENSE
+-rw-r--r--   0        0        0      626 2023-04-24 17:56:47.544492 pysigma_backend_microsoft365defender-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      407 2023-04-24 17:56:47.544492 pysigma_backend_microsoft365defender-0.1.3/sigma/backends/microsoft365defender/__init__.py
+-rw-r--r--   0        0        0    12539 2023-04-24 17:56:47.544492 pysigma_backend_microsoft365defender-0.1.3/sigma/backends/microsoft365defender/microsoft365defender.py
+-rw-r--r--   0        0        0      315 2023-04-24 17:56:47.544492 pysigma_backend_microsoft365defender-0.1.3/sigma/pipelines/microsoft365defender/__init__.py
+-rw-r--r--   0        0        0    29236 2023-04-24 17:56:47.544492 pysigma_backend_microsoft365defender-0.1.3/sigma/pipelines/microsoft365defender/microsoft365defender.py
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 pysigma_backend_microsoft365defender-0.1.3/PKG-INFO
```

### Comparing `pysigma_backend_microsoft365defender-0.1.2/LICENSE` & `pysigma_backend_microsoft365defender-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_microsoft365defender-0.1.2/pyproject.toml` & `pysigma_backend_microsoft365defender-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-microsoft365defender"
-version = "0.1.2"
+version = "0.1.3"
 description = "pySigma Microsoft 365 Defender backend"
 authors = ["Stephen Lincoln <stephen.lincoln@attackiq.com>"]
 license = "LGPL-3.0-only"
 repository = "https://github.com/AttackIQ/pySigma-backend-microsoft365defender"
 packages = [
     { include = "sigma" }
 ]
```

### Comparing `pysigma_backend_microsoft365defender-0.1.2/sigma/backends/microsoft365defender/microsoft365defender.py` & `pysigma_backend_microsoft365defender-0.1.3/sigma/backends/microsoft365defender/microsoft365defender.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,23 +22,23 @@
     formats: Dict[str, str] = {
         "default": "KQL for Microsoft 365 Defender Advanced Hunting queries",
     }
 
     requires_pipeline: bool = False  # m365 pipeline is automatically applied
 
     # Operator precedence
-    precedence: ClassVar[Tuple[ConditionItem, ConditionItem, ConditionItem]] = (ConditionNOT, ConditionOR, ConditionAND)
+    parenthesize = True
+    precedence: ClassVar[Tuple[ConditionItem, ConditionItem, ConditionItem]] = (ConditionNOT, ConditionAND, ConditionOR)
     group_expression: ClassVar[
         str] = "({expr})"  # Expression for precedence override grouping as format string with {expr} placeholder
-
     # Generated query tokens
     token_separator: str = " "  # separator inserted between all boolean operators
     or_token: ClassVar[str] = "or"
     and_token: ClassVar[str] = "and"
-    not_token: ClassVar[str] = " !~ "
+    not_token: ClassVar[str] = "not"
     eq_token: ClassVar[str] = " =~ "  # Token inserted between field and value (without separator)
 
     # String output
     ## Fields
     ### Quoting
     field_quote: ClassVar[
         str] = "'"  # Character used to quote field characters if field_quote_pattern matches (or not, depending on field_quote_pattern_negation). No field name quoting is done if not set.
@@ -105,15 +105,15 @@
     convert_or_as_in: ClassVar[bool] = True  # Convert OR as in-expression
     convert_and_as_in: ClassVar[bool] = True  # Convert AND as in-expression
     in_expressions_allow_wildcards: ClassVar[
         bool] = True  # Values in list can contain wildcards. If set to False (default) only plain values are converted into in-expressions.
     field_in_list_expression: ClassVar[
         str] = "{field} {op} ({list})"  # Expression for field in list of values as format string with placeholders {field}, {op} and {list}
     or_in_operator: ClassVar[
-        str] = "has_any"  # Operator used to convert OR into in-expressions. Must be set if convert_or_as_in is set
+        str] = "in~"  # Operator used to convert OR into in-expressions. Must be set if convert_or_as_in is set
     and_in_operator: ClassVar[
         str] = "has_all"  # Operator used to convert AND into in-expressions. Must be set if convert_and_as_in is set
     list_separator: ClassVar[str] = ", "  # List element separator
 
     # Value not bound to a field
     unbound_value_str_expression: ClassVar[
         str] = '{value}'  # Expression for string value not bound to a field as format string with placeholder {value}
@@ -181,14 +181,31 @@
                 expr = self.convert_condition_field_eq_val_str(new_cond, state)
                 wildcard_exprs_list.append(expr)
         wildcard_exprs = f'{self.token_separator}{op2}{self.token_separator}'.join(wildcard_exprs_list)
         if as_in_expr and wildcard_exprs:
             return as_in_expr + self.token_separator + op2 + self.token_separator + wildcard_exprs
         return as_in_expr + wildcard_exprs
 
+    def convert_condition_not(self, cond: ConditionNOT, state: ConversionState) -> Union[str, DeferredQueryExpression]:
+        """Conversion of NOT conditions. Overridden to surround the group or expr of the 'not' negation with parens,
+        as expected by KQL.
+        """
+        arg = cond.args[0]
+        try:
+            if arg.__class__ in self.precedence:  # group if AND or OR condition is negated
+                return self.not_token + "(" + self.convert_condition_group(arg, state) + ")"
+            else:
+                expr = self.convert_condition(arg, state)
+                if isinstance(expr, DeferredQueryExpression):  # negate deferred expression and pass it to parent
+                    return expr.negate()
+                else:  # convert negated expression to string
+                    return self.not_token + "(" + expr + ")"
+        except TypeError:  # pragma: no cover
+            raise NotImplementedError("Operator 'not' not supported by the backend")
+
     def finalize_query_default(self, rule: SigmaRule, query: Any, index: int, state: ConversionState) -> Any:
         """
         Finalize conversion result of a query. The classes default behavior is to just return the query.
         We will add the table name to the beginning of the query based on the category of the rule.
         This is taken from the ProcessingPipeline state, which is why we automatically run the
         pipeline as part of the backend.
         """
```

### Comparing `pysigma_backend_microsoft365defender-0.1.2/sigma/pipelines/microsoft365defender/microsoft365defender.py` & `pysigma_backend_microsoft365defender-0.1.3/sigma/pipelines/microsoft365defender/microsoft365defender.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_microsoft365defender-0.1.2/PKG-INFO` & `pysigma_backend_microsoft365defender-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-microsoft365defender
-Version: 0.1.2
+Version: 0.1.3
 Summary: pySigma Microsoft 365 Defender backend
 Home-page: https://github.com/AttackIQ/pySigma-backend-microsoft365defender
 License: LGPL-3.0-only
 Author: Stephen Lincoln
 Author-email: stephen.lincoln@attackiq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```


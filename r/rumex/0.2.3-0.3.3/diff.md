# Comparing `tmp/rumex-0.2.3.tar.gz` & `tmp/rumex-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rumex-0.2.3.tar", max compression
+gzip compressed data, was "rumex-0.3.3.tar", max compression
```

## Comparing `rumex-0.2.3.tar` & `rumex-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1211 2022-10-01 01:54:46.296415 rumex-0.2.3/LICENSE
--rw-r--r--   0        0        0     4537 2023-04-04 21:27:51.312254 rumex-0.2.3/README.rst
--rw-r--r--   0        0        0      916 2023-04-04 21:27:51.312254 rumex-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      133 2023-04-04 21:09:15.955235 rumex-0.2.3/rumex/__init__.py
--rw-r--r--   0        0        0        0 2022-10-01 01:54:46.296415 rumex-0.2.3/rumex/parsing/__init__.py
--rw-r--r--   0        0        0     2508 2023-04-04 00:34:13.843051 rumex-0.2.3/rumex/parsing/builder.py
--rw-r--r--   0        0        0      899 2023-04-04 00:34:13.843051 rumex-0.2.3/rumex/parsing/core.py
--rw-r--r--   0        0        0     6958 2023-04-04 21:17:37.959563 rumex-0.2.3/rumex/parsing/parser.py
--rw-r--r--   0        0        0      990 2023-04-04 00:34:13.843051 rumex-0.2.3/rumex/parsing/table.py
--rw-r--r--   0        0        0     2207 2023-04-04 00:34:13.843051 rumex-0.2.3/rumex/parsing/tokenizer.py
--rw-r--r--   0        0        0     9881 2023-04-04 00:34:13.843051 rumex-0.2.3/rumex/runner.py
--rw-r--r--   0        0        0     1553 2023-04-04 00:34:13.843051 rumex-0.2.3/rumex/tests/__init__.py
--rw-r--r--   0        0        0      810 2023-04-04 00:34:13.843051 rumex-0.2.3/rumex/tests/test_error_reporting.py
--rw-r--r--   0        0        0     5554 2023-04-04 00:34:13.843051 rumex-0.2.3/rumex/tests/test_no_execution_cases.py
--rw-r--r--   0        0        0     5022 2023-04-04 00:34:13.843051 rumex-0.2.3/rumex/tests/test_simple_execution.py
--rw-r--r--   0        0        0     3649 2023-04-04 00:34:13.843051 rumex-0.2.3/rumex/tests/test_table.py
--rw-r--r--   0        0        0      894 2023-02-16 02:20:09.255404 rumex-0.2.3/rumex/utils.py
--rw-r--r--   0        0        0     5330 1970-01-01 00:00:00.000000 rumex-0.2.3/setup.py
--rw-r--r--   0        0        0     4817 1970-01-01 00:00:00.000000 rumex-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1211 2022-10-01 01:54:46.296415 rumex-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4537 2023-04-04 21:27:51.312254 rumex-0.3.3/README.rst
+-rw-r--r--   0        0        0      916 2023-04-23 21:55:25.650645 rumex-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-04-23 21:55:25.650645 rumex-0.3.3/rumex/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-01 01:54:46.296415 rumex-0.3.3/rumex/parsing/__init__.py
+-rw-r--r--   0        0        0     3210 2023-04-23 21:55:25.650645 rumex-0.3.3/rumex/parsing/builder.py
+-rw-r--r--   0        0        0      899 2023-04-04 00:34:13.843051 rumex-0.3.3/rumex/parsing/core.py
+-rw-r--r--   0        0        0     7405 2023-04-23 21:55:25.650645 rumex-0.3.3/rumex/parsing/parser.py
+-rw-r--r--   0        0        0      990 2023-04-04 00:34:13.843051 rumex-0.3.3/rumex/parsing/table.py
+-rw-r--r--   0        0        0     2363 2023-04-23 21:55:25.650645 rumex-0.3.3/rumex/parsing/tokenizer.py
+-rw-r--r--   0        0        0     9814 2023-04-23 21:55:25.650645 rumex-0.3.3/rumex/runner.py
+-rw-r--r--   0        0        0     1423 2023-04-23 21:55:25.650645 rumex-0.3.3/rumex/tests/__init__.py
+-rw-r--r--   0        0        0     4206 2023-04-23 21:55:25.650645 rumex-0.3.3/rumex/tests/test_data.py
+-rw-r--r--   0        0        0      810 2023-04-04 00:34:13.843051 rumex-0.3.3/rumex/tests/test_error_reporting.py
+-rw-r--r--   0        0        0     5554 2023-04-04 00:34:13.843051 rumex-0.3.3/rumex/tests/test_no_execution_cases.py
+-rw-r--r--   0        0        0     5022 2023-04-04 00:34:13.843051 rumex-0.3.3/rumex/tests/test_simple_execution.py
+-rw-r--r--   0        0        0      894 2023-02-16 02:20:09.255404 rumex-0.3.3/rumex/utils.py
+-rw-r--r--   0        0        0     5330 1970-01-01 00:00:00.000000 rumex-0.3.3/setup.py
+-rw-r--r--   0        0        0     4817 1970-01-01 00:00:00.000000 rumex-0.3.3/PKG-INFO
```

### Comparing `rumex-0.2.3/LICENSE` & `rumex-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rumex-0.2.3/README.rst` & `rumex-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `rumex-0.2.3/pyproject.toml` & `rumex-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rumex"
-version = "0.2.3"
+version = "0.3.3"
 
 description = ""
 authors = ["uigctaw <uigctaw@metadata.social>"]
 readme = "README.rst"
 
 
 [tool.poetry.dependencies]
```

### Comparing `rumex-0.2.3/rumex/parsing/builder.py` & `rumex-0.3.3/rumex/parsing/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,27 +21,52 @@
         else:
             self._data.append(row)
 
     def get_built(self):
         return tuple(dict(zip(self._header, row)) for row in self._data)
 
 
+class TextBlockBuilder:
+
+    def __init__(self):
+        self._lines = []
+
+    def consume(self, line):
+        self._lines.append(line)
+
+    def get_built(self):
+        return textwrap.dedent('\n'.join(self._lines)).strip()
+
+
 class StepBuilder:
 
     def __init__(self, sentence):
         self.sentence = sentence
-        self._table_builder = TableBuilder()
+        self._builder = None
+        self._table = False
+        self._text_block = False
 
     def add_step_data(self, data):
-        self._table_builder.consume(data)
+        self._table = True
+        if self._text_block:
+            raise AssertionError('Unexpected usage.')
+        self._builder = self._builder or TableBuilder()
+        self._builder.consume(data)
+
+    def add_text_block_line(self, line):
+        self._text_block = True
+        if self._table:
+            raise AssertionError('Unexpected usage.')
+        self._builder = self._builder or TextBlockBuilder()
+        self._builder.consume(line)
 
     def get_built(self):
         return Step(
                 sentence=self.sentence,
-                data=self._table_builder.get_built(),
+                data=self._builder.get_built() if self._builder else None,
         )
 
 
 class ScenarioBuilder:
 
     def __init__(self, name):
         self.name = name
```

### Comparing `rumex-0.2.3/rumex/parsing/core.py` & `rumex-0.3.3/rumex/parsing/core.py`

 * *Files identical despite different names*

### Comparing `rumex-0.2.3/rumex/parsing/parser.py` & `rumex-0.3.3/rumex/parsing/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     """Possible states of the default state machine."""
 
     START = auto()
     FILE_NAME = auto()
     FILE_DESCRIPTION = auto()
     NEW_SCENARIO = auto()
     STEP = auto()
+    BLOCK_OF_TEXT = auto()
     SCENARIO_DESCRIPTION = auto()
 
 
 class StateMachine(Mapping):
     """Represents possible states of a parser.
 
     This object is a map where keys are `State` enumerals
@@ -112,14 +113,19 @@
     builder.current_scenario_builder.description.append(line)
 
 
 def add_step_data(builder, data):
     builder.current_scenario_builder.current_step_builder.add_step_data(data)
 
 
+def add_text_block_line(builder, line):
+    builder.current_scenario_builder.current_step_builder.add_text_block_line(
+            line)
+
+
 default_state_machine = StateMachine({
     State.START: {
         TokenKind.NAME_KW: (State.FILE_NAME, set_file_name),
         TokenKind.BLANK_LINE: (State.START, no_op),
         TokenKind.SCENARIO_KW: (State.NEW_SCENARIO, new_scenario),
         TokenKind.DESCRIPTION: (
             State.FILE_DESCRIPTION, append_file_description),
@@ -169,17 +175,22 @@
             State.SCENARIO_DESCRIPTION, append_scenario_description),
         TokenKind.STEP_KW: (State.STEP, new_step),
     },
 
     State.STEP: {
         TokenKind.STEP_KW: (State.STEP, new_step),
         TokenKind.DESCRIPTION: (State.STEP, add_step_data),
+        TokenKind.TRIPLE_QUOTE: (State.BLOCK_OF_TEXT, no_op),
         TokenKind.BLANK_LINE: (State.STEP, no_op),
     },
 
+    State.BLOCK_OF_TEXT: {
+            kind: (State.BLOCK_OF_TEXT, add_text_block_line)
+            for kind in TokenKind if kind != TokenKind.TRIPLE_QUOTE
+    } | {TokenKind.TRIPLE_QUOTE: (State.NEW_SCENARIO, no_op)},
 })
 
 
 def parse(
         input_file: InputFile,
         *,
         state_machine: StateMachine = default_state_machine,
```

### Comparing `rumex-0.2.3/rumex/parsing/table.py` & `rumex-0.3.3/rumex/parsing/table.py`

 * *Files identical despite different names*

### Comparing `rumex-0.2.3/rumex/parsing/tokenizer.py` & `rumex-0.3.3/rumex/parsing/tokenizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 class TokenKind(Enum):
 
     NAME_KW = auto()
     SCENARIO_KW = auto()
     STEP_KW = auto()
     BLANK_LINE = auto()
     DESCRIPTION = auto()
+    TRIPLE_QUOTE = auto()
 
 
 @dataclass(frozen=True, kw_only=True)
 class Token:
     """Every line must map to a `Token`."""
 
     kind: Hashable
@@ -42,14 +43,19 @@
 
 
 def match_name(line):
     if name := match_keyword('Name', line=line):
         return TokenKind.NAME_KW, name
 
 
+def match_triple_quote(line):
+    if line.strip() == '"""':
+        return TokenKind.TRIPLE_QUOTE, None
+
+
 def match_step(line):
     stripped = line.strip()
     if stripped.startswith(('Given ', 'When ', 'Then ', 'And ')):
         return TokenKind.STEP_KW, line
 
 
 def match_blank_line(line):
@@ -78,14 +84,15 @@
     def __len__(self):
         return len(self._fns)
 
 
 default_tokenizers = Tokenizers(
     match_name,
     match_scenario,
+    match_triple_quote,
     match_step,
     match_blank_line,
     match_description,
 )
 
 
 def iter_tokens(text, tokenizers=default_tokenizers):
```

### Comparing `rumex-0.2.3/rumex/runner.py` & `rumex-0.3.3/rumex/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from typing import Any, Callable, Protocol, TypeAlias
 import inspect
 import re
 
 from .parsing.core import InputFile, File, ParserProto, Scenario
 from .parsing.parser import parse
 
-_STEP_DATA_KWARG = 'step_data'
-
 
 class HookAlreadyRegistered(Exception):
     pass
 
 
 @dataclass(frozen=True, kw_only=True)
 class _ExecutedStep:
@@ -331,20 +329,20 @@
         Decorator for registering a function as a step.
         """
         return lambda fn: self._add_step_fn(fn, pattern=pattern)
 
     def _add_step_fn(self, fn, /, *, pattern):
         self._pattern_to_fn[re.compile(pattern)] = fn
 
-    def _wrap_mapped_function(self, *, fn_spec, fn, mapped_args, step_data):
+    def _wrap_mapped_function(self, *, fn_spec, fn, mapped_args, data):
 
         def wrapped(context):
             kwargs = {}
-            if _STEP_DATA_KWARG in fn_spec.kwonlyargs:
-                kwargs[_STEP_DATA_KWARG] = step_data
+            if 'data' in fn_spec.kwonlyargs:
+                kwargs['data'] = data
             if 'context' in fn_spec.kwonlyargs:
                 kwargs['context'] = context
             return fn(*mapped_args, **kwargs)
 
         return wrapped
 
     def _prepare_step(self, step_):
@@ -357,15 +355,15 @@
                     spec.annotations.get(name, lambda x: x)(value)
                     for name, value in zip(spec.args, args)
                 ]
                 return self._wrap_mapped_function(
                     fn_spec=spec,
                     fn=fn,
                     mapped_args=mapped_args,
-                    step_data=step_.data,
+                    data=step_.data,
                     )
         raise Exception('TODO')
 
     def iter_steps(self, scenario: Scenario) -> Iterable[ExecutableStep]:
         """See documentation of `StepMapperProto`."""
         if (hook := self._hooks.run_before_scenario):
             yield ExecutableStep(sentence=hook.name, callable_=hook.fn)
```

### Comparing `rumex-0.2.3/rumex/tests/__init__.py` & `rumex-0.3.3/rumex/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,15 +52,12 @@
                 steps=steps,
                 context_maker=context_maker,
                 parser=parser,
                 executor=executor,
                 reporter=reporter,
                 map_=map_,
         )
-    try:
-        test(
-                parse=parse,
-                get_step_mapper=get_step_mapper,
-                run=wrapped_run,
-        )
-    except Exception as exc:
-        raise type(exc)(test.__module__ + '.' + test.__name__) from exc
+    test(
+            parse=parse,
+            get_step_mapper=get_step_mapper,
+            run=wrapped_run,
+    )
```

### Comparing `rumex-0.2.3/rumex/tests/test_error_reporting.py` & `rumex-0.3.3/rumex/tests/test_error_reporting.py`

 * *Files identical despite different names*

### Comparing `rumex-0.2.3/rumex/tests/test_no_execution_cases.py` & `rumex-0.3.3/rumex/tests/test_no_execution_cases.py`

 * *Files identical despite different names*

### Comparing `rumex-0.2.3/rumex/tests/test_simple_execution.py` & `rumex-0.3.3/rumex/tests/test_simple_execution.py`

 * *Files identical despite different names*

### Comparing `rumex-0.2.3/rumex/tests/test_table.py` & `rumex-0.3.3/rumex/tests/test_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -60,16 +60,16 @@
             | ab cd | AB CD |
             | efgh  |   UVW |
     ''')
     reporter = Reporter()
     steps = get_step_mapper()
 
     @steps(r'Given the following stuff:')
-    def given_(*, step_data):
-        assert step_data == (
+    def given_(*, data):
+        assert data == (
                 {'Col 1': 'ab cd', 'Col 2': 'AB CD'},
                 {'Col 1': 'efgh', 'Col 2': 'UVW'},
         )
 
     run(
         files=[InputFile(uri='we', text=text)],
         reporter=reporter,
@@ -90,16 +90,16 @@
             | ab\|cd  |   AB CD\\ |
             | efgh\   | \| UVW \| |
     ''')
     reporter = Reporter()
     steps = get_step_mapper()
 
     @steps(r'Given the following stuff:')
-    def given_(*, step_data):
-        assert step_data == (
+    def given_(*, data):
+        assert data == (
                 {'Col |1': 'ab|cd', 'Col| 2': 'AB CD\\'},
                 {'Col |1': 'efgh', 'Col| 2': '| UVW |'},
         )
 
     run(
         files=[InputFile(uri='we', text=text)],
         reporter=reporter,
@@ -124,26 +124,53 @@
             +-------+-------+
             | baz   | qux   |
     ''')
     reporter = Reporter()
     steps = get_step_mapper()
 
     @steps(r'Given the following stuff:')
-    def given_(*, step_data):
-        assert step_data == (
+    def given_(*, data):
+        assert data == (
                 {'Col 1': 'foo', 'Col 2': 'bar'},
         )
 
     @steps(r'Given this stuff:')
-    def given_2(*, step_data):
-        assert step_data == (
+    def given_2(*, data):
+        assert data == (
                 {'Col a': 'baz', 'Col b': 'qux'},
         )
 
     run(
         files=[InputFile(uri='we', text=text)],
         reporter=reporter,
         steps=steps,
     )
 
+    executed_file, = reporter.reported
+    assert executed_file.success
+
+
+def test_steps_with_a_block_of_text(get_step_mapper, run, **_):
+    text = textwrap.dedent('''
+        Scenario: Steps with text
+
+        Given the following stuff:
+            """
+            Hello!
+                Hi!
+            """
+    ''')
+    reporter = Reporter()
+    steps = get_step_mapper()
+
+    @steps(r'Given the following stuff:')
+    def given_(*, data):
+        assert data == 'Hello!\n    Hi!'
+
+    run(
+        files=[InputFile(uri='we', text=text)],
+        reporter=reporter,
+        steps=steps,
+    )
+
     executed_file, = reporter.reported
     assert executed_file.success
```

### Comparing `rumex-0.2.3/rumex/utils.py` & `rumex-0.3.3/rumex/utils.py`

 * *Files identical despite different names*

### Comparing `rumex-0.2.3/setup.py` & `rumex-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['rumex', 'rumex.parsing', 'rumex.tests']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'rumex',
-    'version': '0.2.3',
+    'version': '0.3.3',
     'description': '',
     'long_description': '=====\nRumex\n=====\n\n`Behaviour Driven Development`_ (BDD) testing library.\n\nRumex is a lightweight library alternative to the `behave`_ framework.\n\n\nBasic example\n-------------\n\n.. code:: python\n\n    import rumex\n\n    example_file = rumex.InputFile(\n        text=\'\'\'\n            Name: Basic example\n\n            Scenario: Simple arithmetics\n\n                Given an integer 1\n                And an integer 2\n                When addition is performed\n                Then the result is 3\n        \'\'\',\n        uri=\'in place file, just an example\',\n    )\n\n    steps = rumex.StepMapper()\n\n\n    class Context:\n\n        def __init__(self):\n            self.integers = []\n            self.sum = None\n\n\n    @steps(r\'an integer (\\d+)\')\n    def store_integer(integer: int, *, context: Context):\n        context.integers.append(integer)\n\n\n    @steps(r\'addition is performed\')\n    def add(*, context: Context):\n        context.sum = sum(context.integers)\n\n\n    @steps(r\'the result is (\\d+)\')\n    def check_result(expected_result: int, *, context: Context):\n        assert expected_result == context.sum\n\n\n    rumex.run(\n        files=[example_file],\n        steps=steps,\n        context_maker=Context,\n    )\n\n\nMore examples\n~~~~~~~~~~~~~\n\nSee `docs/examples`_\n\n\nAPI\n---\n\nFor complete API documentation see `docs/api`_\n\nrumex.run\n~~~~~~~~~\n\n.. code::\n\n    rumex.run(\n        *,\n        files: Iterable[InputFile],\n        steps: StepMapperProto,\n        context_maker: Callable[[], Any] | None = None,\n        parser: ParserProto = rumex.parsing.parser.parse,\n        executor: ExecutorProto = rumex.runner.execute_file,\n        reporter=rumex.runner.report,\n        map_=builtins.map\n    )\n\nRumex entry point for running tests.\n\n.. rubric:: Parameters\n\n- files: Files to be parsed and executed.\n- steps: See `StepMapper` or `StepMapperProto` for more info.\n- context_maker: A callable that returns an object that can be passed to step functions.\n- parser: A callable that takes `InputFile` and returns `File`.\n- executor: A callable that takes `File` `steps` and `context_maker` and returns `ExecutedFile`.\n- reporter: A callable that takes the collection of all executed files. This can be as simple as raising an exception if any of the executed files is a `FailedFile`.\n- map\\_: Must have the same interface as the Python\'s built-in `map`. Custom implementation might be used to speed up file parsing or execution.\n\nrumex.InputFile\n~~~~~~~~~~~~~~~\n\nFrozen dataclass\n\n.. code::\n\n    rumex.InputFile(\n        *,\n        uri: str,\n        text: str\n    )\n\nContainer for a test file to be parsed.\n\nDoes not have to represent an actual file.\nCould be e.g. an entry in a database.\n\n.. rubric:: Parameters\n\n- uri: A unique identifer. If it\'s a file, this could be a path to this file.\n- text: The content of the file.\n\nrumex.StepMapper\n~~~~~~~~~~~~~~~~\n\nPrepare step functions.\n\nMethods\n.......\n\n:\n\n----\n\n.. code::\n\n    before_scenario(\n        self,\n        callable_: ContextCallable,\n        /\n    )\n\nRegister a function to execute at the start of each scenario.\n\n.. rubric:: Parameters\n\n- callable\\_: The function to be executed.\n\n----\n\n.. code::\n\n    before_step(\n        self,\n        callable_: ContextCallable,\n        /\n    )\n\nRegister a function to execute before each step.\n\n.. rubric:: Parameters\n\n- callable\\_: The function to be executed.\n\n----\n\n.. code::\n\n    __call__(\n        self,\n        pattern: str\n    )\n\nCreate decorator for registering steps.\n\nFor example, to register a function:\n\n.. code:: python\n\n    def say_hello(person, *, context): ...\n\n\nto match sentence "Then Bob says hello",\nyou can do:\n\n.. code:: python\n\n        steps = StepMapper()\n\n        @steps(r\'(\\w+) says hello\')\n        def say_hello(person, *, context):\n            context.get_person(person).say(\'hello\')\n\n\n.. rubric:: Parameters\n\n- pattern: Regex pattern that will be used to match a sentence.\n\n----\n\n.. code::\n\n    iter_steps(\n        self,\n        scenario: Scenario\n    )\n\nSee documentation of `StepMapperProto`.\n\n\n\n\nrumex.find_input_files\n~~~~~~~~~~~~~~~~~~~~~~\n\n.. code::\n\n    rumex.find_input_files(\n        *,\n        root: Path,\n        extension: str\n    )\n\nFind regular files and return them as `InputFile[s]`.\n\n.. rubric:: Parameters\n\n- root: Where to start searching recursively.\n- extension: Extension of the files to look for.\n\n\n.. _`Behaviour Driven Development`:\n  https://en.wikipedia.org/wiki/Behavior-driven_development\n\n.. _`behave`: https://github.com/behave/behave\n\n.. _`docs/examples`: docs/examples\n\n.. _`docs/api`: docs/api.rst\n',
     'author': 'uigctaw',
     'author_email': 'uigctaw@metadata.social',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `rumex-0.2.3/PKG-INFO` & `rumex-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rumex
-Version: 0.2.3
+Version: 0.3.3
 Summary: 
 Author: uigctaw
 Author-email: uigctaw@metadata.social
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
```


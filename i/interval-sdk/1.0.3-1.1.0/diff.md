# Comparing `tmp/interval_sdk-1.0.3.tar.gz` & `tmp/interval_sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interval_sdk-1.0.3.tar", max compression
+gzip compressed data, was "interval_sdk-1.1.0.tar", max compression
```

## Comparing `interval_sdk-1.0.3.tar` & `interval_sdk-1.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     2968 2023-02-09 22:23:52.939868 interval_sdk-1.0.3/README.md
--rw-r--r--   0        0        0     1890 2023-04-20 18:41:38.393235 interval_sdk-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      331 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/classes/__init__.py
--rw-r--r--   0        0        0      422 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/classes/action.py
--rw-r--r--   0        0        0     7024 2023-04-20 18:40:02.490552 interval_sdk-1.0.3/src/interval_sdk/classes/component.py
--rw-r--r--   0        0        0      931 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/classes/interval_file.py
--rw-r--r--   0        0        0    57635 2023-04-20 18:41:38.393235 interval_sdk-1.0.3/src/interval_sdk/classes/io.py
--rw-r--r--   0        0        0     8151 2023-04-20 18:40:02.490552 interval_sdk-1.0.3/src/interval_sdk/classes/io_client.py
--rw-r--r--   0        0        0      348 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/classes/io_error.py
--rw-r--r--   0        0        0    35098 2023-04-20 18:40:02.493885 interval_sdk-1.0.3/src/interval_sdk/classes/io_promise.py
--rw-r--r--   0        0        0     7891 2023-04-20 18:40:02.493885 interval_sdk-1.0.3/src/interval_sdk/classes/isocket.py
--rw-r--r--   0        0        0     1290 2023-04-14 17:16:59.713107 interval_sdk-1.0.3/src/interval_sdk/classes/layout.py
--rw-r--r--   0        0        0     3458 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/classes/logger.py
--rw-r--r--   0        0        0     2993 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/classes/page.py
--rw-r--r--   0        0        0     6155 2023-04-20 18:40:02.493885 interval_sdk-1.0.3/src/interval_sdk/classes/rpc.py
--rw-r--r--   0        0        0     2968 2023-03-27 15:09:45.572798 interval_sdk-1.0.3/src/interval_sdk/classes/transaction_loading_state.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/components/__init__.py
--rw-r--r--   0        0        0     1704 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/components/grid.py
--rw-r--r--   0        0        0     6090 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/components/table.py
--rw-r--r--   0        0        0      810 2023-04-20 18:40:02.493885 interval_sdk-1.0.3/src/interval_sdk/handlers.py
--rw-r--r--   0        0        0    13589 2023-04-20 18:40:02.493885 interval_sdk-1.0.3/src/interval_sdk/internal_rpc_schema.py
--rw-r--r--   0        0        0    25561 2023-04-17 13:45:05.449358 interval_sdk-1.0.3/src/interval_sdk/io_schema.py
--rw-r--r--   0        0        0    56972 2023-04-20 18:40:02.493885 interval_sdk-1.0.3/src/interval_sdk/main.py
--rw-r--r--   0        0        0       41 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/superjson/__init__.py
--rw-r--r--   0        0        0     1081 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/superjson/main.py
--rw-r--r--   0        0        0     3810 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/superjson/plainer.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/superjson/tests/__init__.py
--rw-r--r--   0        0        0      188 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/superjson/tests/node-only-types.js
--rw-r--r--   0        0        0      416 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/superjson/tests/round-trip-superjson.js
--rw-r--r--   0        0        0     3385 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/superjson/tests/test_superjson.py
--rw-r--r--   0        0        0     5790 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/superjson/transformer.py
--rw-r--r--   0        0        0     4550 2023-04-14 17:16:59.716440 interval_sdk-1.0.3/src/interval_sdk/types.py
--rw-r--r--   0        0        0     7193 2023-04-14 17:16:59.716440 interval_sdk-1.0.3/src/interval_sdk/util.py
--rw-r--r--   0        0        0     4207 1970-01-01 00:00:00.000000 interval_sdk-1.0.3/setup.py
--rw-r--r--   0        0        0     4051 1970-01-01 00:00:00.000000 interval_sdk-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2968 2023-02-09 22:23:52.939868 interval_sdk-1.1.0/README.md
+-rw-r--r--   0        0        0     1890 2023-04-24 18:28:48.134160 interval_sdk-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      331 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/classes/__init__.py
+-rw-r--r--   0        0        0      422 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/classes/action.py
+-rw-r--r--   0        0        0     7024 2023-04-20 18:40:02.490552 interval_sdk-1.1.0/src/interval_sdk/classes/component.py
+-rw-r--r--   0        0        0      931 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/classes/interval_file.py
+-rw-r--r--   0        0        0    57635 2023-04-24 17:19:39.837392 interval_sdk-1.1.0/src/interval_sdk/classes/io.py
+-rw-r--r--   0        0        0     8151 2023-04-20 18:40:02.490552 interval_sdk-1.1.0/src/interval_sdk/classes/io_client.py
+-rw-r--r--   0        0        0      348 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/classes/io_error.py
+-rw-r--r--   0        0        0    35098 2023-04-20 18:40:02.493885 interval_sdk-1.1.0/src/interval_sdk/classes/io_promise.py
+-rw-r--r--   0        0        0     7891 2023-04-24 17:19:39.837392 interval_sdk-1.1.0/src/interval_sdk/classes/isocket.py
+-rw-r--r--   0        0        0     1290 2023-04-14 17:16:59.713107 interval_sdk-1.1.0/src/interval_sdk/classes/layout.py
+-rw-r--r--   0        0        0     3458 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/classes/logger.py
+-rw-r--r--   0        0        0     2993 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/classes/page.py
+-rw-r--r--   0        0        0     6155 2023-04-24 17:19:39.837392 interval_sdk-1.1.0/src/interval_sdk/classes/rpc.py
+-rw-r--r--   0        0        0     2968 2023-03-27 15:09:45.572798 interval_sdk-1.1.0/src/interval_sdk/classes/transaction_loading_state.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/components/__init__.py
+-rw-r--r--   0        0        0     1704 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/components/grid.py
+-rw-r--r--   0        0        0     6173 2023-04-24 17:47:34.117311 interval_sdk-1.1.0/src/interval_sdk/components/table.py
+-rw-r--r--   0        0        0      810 2023-04-20 18:40:02.493885 interval_sdk-1.1.0/src/interval_sdk/handlers.py
+-rw-r--r--   0        0        0    15208 2023-04-24 17:30:45.828290 interval_sdk-1.1.0/src/interval_sdk/internal_rpc_schema.py
+-rw-r--r--   0        0        0    25774 2023-04-24 17:47:34.107311 interval_sdk-1.1.0/src/interval_sdk/io_schema.py
+-rw-r--r--   0        0        0    65147 2023-04-24 18:36:10.017979 interval_sdk-1.1.0/src/interval_sdk/main.py
+-rw-r--r--   0        0        0       41 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/superjson/__init__.py
+-rw-r--r--   0        0        0     1081 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/superjson/main.py
+-rw-r--r--   0        0        0     3810 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/superjson/plainer.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/superjson/tests/__init__.py
+-rw-r--r--   0        0        0      188 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/superjson/tests/node-only-types.js
+-rw-r--r--   0        0        0      416 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/superjson/tests/round-trip-superjson.js
+-rw-r--r--   0        0        0     3385 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/superjson/tests/test_superjson.py
+-rw-r--r--   0        0        0     5790 2023-02-09 22:23:52.943201 interval_sdk-1.1.0/src/interval_sdk/superjson/transformer.py
+-rw-r--r--   0        0        0     4550 2023-04-14 17:16:59.716440 interval_sdk-1.1.0/src/interval_sdk/types.py
+-rw-r--r--   0        0        0     7193 2023-04-14 17:16:59.716440 interval_sdk-1.1.0/src/interval_sdk/util.py
+-rw-r--r--   0        0        0     4207 1970-01-01 00:00:00.000000 interval_sdk-1.1.0/setup.py
+-rw-r--r--   0        0        0     4051 1970-01-01 00:00:00.000000 interval_sdk-1.1.0/PKG-INFO
```

### Comparing `interval_sdk-1.0.3/README.md` & `interval_sdk-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/pyproject.toml` & `interval_sdk-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interval-sdk"
-version = "1.0.3"
+version = "1.1.0"
 description = "The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more."
 authors = [
 	"Jacob Mischka <jacob@interval.com>",
 	"Ryan Coppolo <ryan@interval.com>",
 ]
 maintainers = [
 	"Jacob Mischka <jacob@interval.com>",
```

### Comparing `interval_sdk-1.0.3/src/interval_sdk/classes/component.py` & `interval_sdk-1.1.0/src/interval_sdk/classes/component.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/classes/interval_file.py` & `interval_sdk-1.1.0/src/interval_sdk/classes/interval_file.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/classes/io.py` & `interval_sdk-1.1.0/src/interval_sdk/classes/io.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/classes/io_client.py` & `interval_sdk-1.1.0/src/interval_sdk/classes/io_client.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/classes/io_promise.py` & `interval_sdk-1.1.0/src/interval_sdk/classes/io_promise.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/classes/isocket.py` & `interval_sdk-1.1.0/src/interval_sdk/classes/isocket.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/classes/layout.py` & `interval_sdk-1.1.0/src/interval_sdk/classes/layout.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/classes/logger.py` & `interval_sdk-1.1.0/src/interval_sdk/classes/logger.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/classes/page.py` & `interval_sdk-1.1.0/src/interval_sdk/classes/page.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/classes/rpc.py` & `interval_sdk-1.1.0/src/interval_sdk/classes/rpc.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/classes/transaction_loading_state.py` & `interval_sdk-1.1.0/src/interval_sdk/classes/transaction_loading_state.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/components/grid.py` & `interval_sdk-1.1.0/src/interval_sdk/components/grid.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/components/table.py` & `interval_sdk-1.1.0/src/interval_sdk/components/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,22 @@
 
 def columns_builder(
     data: Optional[Union[Iterable[TableRow], Any]] = None,
     columns: Optional[Iterable[Union[TableColumnDef, str]]] = None,
     log_missing_column: Optional[Callable[[str], None]] = None,
 ) -> list[TableColumnDef]:
     # using a dict instead of a set because dicts are ordered and sets aren't
-    data_columns: dict[str, None] = (
-        {col: None for row in data for col in row.keys()} if data is not None else {}
-    )
+    try:
+        data_columns: dict[str, None] = (
+            {col: None for row in data for col in row.keys()}
+            if data is not None
+            else {}
+        )
+    except:
+        data_columns = {}
 
     if columns:
 
         def normalize_col(col: Union[TableColumnDef, str]) -> TableColumnDef:
             if isinstance(col, str):
                 col = cast(str, col)
```

### Comparing `interval_sdk-1.0.3/src/interval_sdk/handlers.py` & `interval_sdk-1.1.0/src/interval_sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/internal_rpc_schema.py` & `interval_sdk-1.1.0/src/interval_sdk/internal_rpc_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 
 
 class SendRedirectInputs(BaseModel):
     transaction_id: str
     url: Optional[str] = None
     route: Optional[str] = None
     params: Optional[SerializableRecord] = None
+    replace: Optional[bool] = None
 
 
 class MarkTransactionCompleteInputs(BaseModel):
     transaction_id: str
     result: Optional[str]
 
 
@@ -461,14 +462,15 @@
         )
 
     async def redirect(
         self,
         url: Optional[str] = None,
         route: Optional[str] = None,
         params: Optional[SerializableRecord] = None,
+        replace: Optional[bool] = None,
     ):
         if (url is None and route is None) or (url is not None and route is not None):
             self._logger.error("Must specify exactly one of either `url` or `route`.")
 
         inputs = SendRedirectInputs(
             transaction_id=self._transaction_id,
         )
@@ -476,30 +478,83 @@
         if url is not None:
             inputs.url = url
         if route is not None:
             inputs.route = route
             if params is not None:
                 inputs.params = params
 
+        if replace is not None:
+            inputs.replace = replace
+
         await self._send_redirect(inputs)
 
 
 @dataclass
 class PageInfo:
     slug: str
 
 
-@dataclass
 class PageContext:
     environment: ActionEnvironment
     user: ContextUser
     params: SerializableRecord
     organization: OrganizationDef
     page: PageInfo
 
+    _page_key: str
+    _logger: Logger
+    _send_redirect: Callable[[SendRedirectInputs], Awaitable[None]]
+
+    def __init__(
+        self,
+        page_key: str,
+        logger: Logger,
+        environment: ActionEnvironment,
+        user: ContextUser,
+        params: SerializableRecord,
+        organization: OrganizationDef,
+        page: PageInfo,
+        send_redirect: Callable[[SendRedirectInputs], Awaitable[None]],
+    ):
+        self._page_key = page_key
+        self._logger = logger
+        self._send_redirect = send_redirect
+
+        self.environment = environment
+        self.user = user
+        self.params = params
+        self.organization = organization
+        self.page = page
+
+    async def redirect(
+        self,
+        url: Optional[str] = None,
+        route: Optional[str] = None,
+        params: Optional[SerializableRecord] = None,
+        replace: Optional[bool] = None,
+    ):
+        if (url is None and route is None) or (url is not None and route is not None):
+            self._logger.error("Must specify exactly one of either `url` or `route`.")
+
+        inputs = SendRedirectInputs(
+            transaction_id=self._page_key,
+        )
+
+        if url is not None:
+            inputs.url = url
+        if route is not None:
+            inputs.route = route
+            if params is not None:
+                inputs.params = params
+
+        if replace is not None:
+            inputs.replace = replace
+
+        await self._send_redirect(inputs)
+
 
 class StartTransactionInputs(BaseModel):
     transaction_id: str
     display_resolves_immediately: bool = False
     action: ActionInfo
     environment: ActionEnvironment
     user: ContextUserModel
```

### Comparing `interval_sdk-1.0.3/src/interval_sdk/io_schema.py` & `interval_sdk-1.1.0/src/interval_sdk/io_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,31 +343,37 @@
     SearchResultValuePrimitive, Mapping[str, SearchResultValuePrimitive], TypedDict
 ]
 
 PassthroughSearchResultValue = TypeVar(
     "PassthroughSearchResultValue", bound=SearchResultValue
 )
 
+HighlightColor: TypeAlias = Literal[
+    "red", "orange", "yellow", "green", "blue", "purple", "pink", "gray"
+]
+
 
 class TableRowValueObject(TypedDict):
     label: NotRequired[TableRowValuePrimitive]
     value: NotRequired[TableRowValuePrimitive]
     url: NotRequired[str]
     route: NotRequired[str]
     params: NotRequired[SerializableRecord]
     image: NotRequired[ImageDefinition]
+    highlightColor: NotRequired[HighlightColor]
 
 
 class TableRowValueObjectModel(BaseModel):
     label: Optional[TableRowValuePrimitive] = None
     value: Optional[TableRowValuePrimitive] = None
     url: Optional[str] = None
     route: Optional[str] = None
     params: Optional[SerializableRecordModel] = None
     image: Optional[ImageDefinitionModel] = None
+    highlightColor: Optional[HighlightColor] = None
 
 
 TableRowValue: TypeAlias = Union[TableRowValueObject, TableRowValuePrimitive]
 TableRow: TypeAlias = Mapping[str, TableRowValue]
 
 
 class TableMenuItem(TypedDict):
```

### Comparing `interval_sdk-1.0.3/src/interval_sdk/main.py` & `interval_sdk-1.1.0/src/interval_sdk/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,25 @@
 
 try:
     sdk_version = importlib.metadata.version(__package__)
 except:
     pass
 
 
+@dataclass
+class IntervalErrorProps:
+    error: BaseException
+    route: str
+    route_definition: Union[Action, Page, None]
+    environment: ActionEnvironment
+    user: ContextUser
+    params: SerializableRecord
+    organization: OrganizationDef
+
+
 class Interval:
     class Routes:
         _interval: "Interval"
 
         def __init__(self, interval: "Interval"):
             self._interval = interval
 
@@ -168,14 +179,15 @@
     environment: Optional[ActionEnvironment] = None
 
     _routes: dict[str, Union[Action, Page]]
     _action_definitions: list[ActionDefinition]
     _page_definitions: list[PageDefinition]
     _action_handlers: dict[str, IntervalActionHandler]
     _page_handlers: dict[str, IntervalPageHandler]
+    _on_error: Optional[Callable[[IntervalErrorProps], None]]
 
     def __init__(
         self,
         api_key: str,
         *,
         endpoint: Optional[str] = None,
         log_level: LogLevel = "info",
@@ -183,14 +195,15 @@
         max_resend_attempts: int = 10,
         send_timeout: float = 5,
         ping_timeout: float = 5,
         ping_interval: float = 30,
         close_unresponsive_connection_timeout: float = 180,
         reinitialize_batch_timeout: float = 0.2,
         num_message_producers: int = 1,
+        on_error: Optional[Callable[[IntervalErrorProps], None]] = None,
     ):
         self._api_key = api_key
         if endpoint is not None:
             self._endpoint = endpoint
 
         url = urlparse(self._endpoint)
         self._http_endpoint = urlunparse(
@@ -215,14 +228,16 @@
         self._pending_page_layouts = {}
         self._transaction_loading_states = {}
         self._routes = {}
         self._action_definitions = []
         self._page_definitions = []
         self._action_handlers = {}
         self._page_handlers = {}
+        self._on_error = on_error
+
         self._logger = Logger(log_level=log_level, prefix=self.__class__.__name__)
         self.routes = Interval.Routes(self)
 
     def _get_api_address(self, path: str) -> str:
         if path.startswith("/"):
             path = path[1:]
 
@@ -928,15 +943,15 @@
                             resp = await handler()  # type: ignore
                         elif len(params) == 1:
                             resp = await handler(client.io)  # type: ignore
                         elif len(params) == 2:
                             resp = await handler(client.io, action_ctx)  # type: ignore
                         else:
                             raise IntervalError(
-                                "handler accepts invalid number of arguments"
+                                "Handler accepts invalid number of arguments"
                             )
 
                         if resp is not None and not isinstance(
                             resp,
                             (
                                 bool,
                                 int,
@@ -957,14 +972,29 @@
                             meta=meta,
                         )
                     except IOError as ioerr:
                         raise ioerr
                     except Exception as err:
                         self._log.error("Error in action handler", err)
                         self._log.print_exception(err)
+                        if self._on_error is not None:
+                            self._on_error(
+                                IntervalErrorProps(
+                                    error=err,
+                                    route=inputs.action.slug,
+                                    route_definition=self._routes.get(
+                                        inputs.action.slug, None
+                                    ),
+                                    environment=action_ctx.environment,
+                                    user=action_ctx.user,
+                                    params=action_ctx.params,
+                                    organization=action_ctx.organization,
+                                )
+                            )
+
                         result = ActionResult(
                             status="FAILURE",
                             data=IOFunctionReturnModel.parse_obj(
                                 {
                                     "error": err.__class__.__name__,
                                     "message": str(err),
                                 }
@@ -1032,19 +1062,22 @@
                 return OpenPageReturnsError(message="No page handler found.")
 
             params = inputs.params
             if params is not None and inputs.params_meta is not None:
                 params = superjson.deserialize(params, inputs.params_meta)
 
             page_ctx = PageContext(
+                page_key=inputs.page_key,
+                logger=self._logger,
                 user=inputs.user,
                 params=deserialize_dates(inputs.params),
                 environment=inputs.environment,
                 organization=self.organization,
                 page=inputs.page,
+                send_redirect=self._send_redirect,
             )
 
             page: Optional[Layout] = None
             menu_items: Optional[list[ButtonItemModel]] = None
             render_instruction: Optional[IORender] = None
             errors: list[PageError] = []
 
@@ -1163,14 +1196,28 @@
 
                     if page.title is not None:
                         if isfunction(page.title):
                             try:
                                 page.title = page.title()
                             except Exception as err:
                                 self._logger.error(err)
+                                if self._on_error is not None:
+                                    self._on_error(
+                                        IntervalErrorProps(
+                                            error=err,
+                                            route=inputs.page.slug,
+                                            route_definition=self._routes.get(
+                                                inputs.page.slug, None
+                                            ),
+                                            environment=page_ctx.environment,
+                                            user=page_ctx.user,
+                                            params=page_ctx.params,
+                                            organization=page_ctx.organization,
+                                        )
+                                    )
                                 errors.append(page_error(err, "title"))
 
                         if iscoroutine(page.title):
                             title_task = loop.create_task(page.title)
 
                             def handle_title(task: asyncio.Task[str]):
                                 nonlocal send_page_task
@@ -1181,14 +1228,29 @@
 
                                 if page is None:
                                     return
 
                                 try:
                                     page.title = task.result()
                                 except Exception as err:
+                                    self._logger.error(err)
+                                    if self._on_error is not None:
+                                        self._on_error(
+                                            IntervalErrorProps(
+                                                error=err,
+                                                route=inputs.page.slug,
+                                                route_definition=self._routes.get(
+                                                    inputs.page.slug, None
+                                                ),
+                                                environment=page_ctx.environment,
+                                                user=page_ctx.user,
+                                                params=page_ctx.params,
+                                                organization=page_ctx.organization,
+                                            )
+                                        )
                                     errors.append(page_error(err, "description"))
 
                                 if send_page_task is None:
                                     send_page_task = loop.create_task(send_page())
                                     send_page_task.add_done_callback(on_page_sent)
 
                             title_task.add_done_callback(handle_title)
@@ -1196,14 +1258,28 @@
 
                     if page.description is not None:
                         if isfunction(page.description):
                             try:
                                 page.description = page.description()
                             except Exception as err:
                                 self._logger.error(err)
+                                if self._on_error is not None:
+                                    self._on_error(
+                                        IntervalErrorProps(
+                                            error=err,
+                                            route=inputs.page.slug,
+                                            route_definition=self._routes.get(
+                                                inputs.page.slug, None
+                                            ),
+                                            environment=page_ctx.environment,
+                                            user=page_ctx.user,
+                                            params=page_ctx.params,
+                                            organization=page_ctx.organization,
+                                        )
+                                    )
                                 errors.append(page_error(err, "description"))
 
                         if iscoroutine(page.description):
                             desc_task = loop.create_task(page.description)
 
                             def handle_desc(task: asyncio.Task[str]):
                                 nonlocal send_page_task
@@ -1214,14 +1290,29 @@
 
                                 if page is None:
                                     return
 
                                 try:
                                     page.description = task.result()
                                 except Exception as err:
+                                    self._logger.error(err)
+                                    if self._on_error is not None:
+                                        self._on_error(
+                                            IntervalErrorProps(
+                                                error=err,
+                                                route=inputs.page.slug,
+                                                route_definition=self._routes.get(
+                                                    inputs.page.slug, None
+                                                ),
+                                                environment=page_ctx.environment,
+                                                user=page_ctx.user,
+                                                params=page_ctx.params,
+                                                organization=page_ctx.organization,
+                                            )
+                                        )
                                     errors.append(page_error(err, "description"))
                                 if send_page_task is None:
                                     send_page_task = loop.create_task(send_page())
                                     send_page_task.add_done_callback(on_page_sent)
 
                             desc_task.add_done_callback(handle_desc)
                             self._page_futures[desc_task.get_name()] = desc_task
@@ -1249,35 +1340,77 @@
                                 task.result()
                                 self._logger.debug(
                                     "Initial children render complete for page_key",
                                     inputs.page_key,
                                 )
                             except IOError as err:
                                 self._logger.error(err)
+                                if self._on_error is not None:
+                                    self._on_error(
+                                        IntervalErrorProps(
+                                            error=err,
+                                            route=inputs.page.slug,
+                                            route_definition=self._routes.get(
+                                                inputs.page.slug, None
+                                            ),
+                                            environment=page_ctx.environment,
+                                            user=page_ctx.user,
+                                            params=page_ctx.params,
+                                            organization=page_ctx.organization,
+                                        )
+                                    )
                                 if err.__cause__ is not None:
                                     errors.append(
                                         page_error(err.__cause__, layout_key="children")
                                     )
                                 else:
                                     errors.append(page_error(err, "children"))
 
                                 if send_page_task is None:
                                     send_page_task = loop.create_task(send_page())
                                     send_page_task.add_done_callback(on_page_sent)
                             except Exception as err:
                                 self._logger.error(err)
+                                if self._on_error is not None:
+                                    self._on_error(
+                                        IntervalErrorProps(
+                                            error=err,
+                                            route=inputs.page.slug,
+                                            route_definition=self._routes.get(
+                                                inputs.page.slug, None
+                                            ),
+                                            environment=page_ctx.environment,
+                                            user=page_ctx.user,
+                                            params=page_ctx.params,
+                                            organization=page_ctx.organization,
+                                        )
+                                    )
                                 errors.append(page_error(err, layout_key="children"))
                                 if send_page_task is None:
                                     send_page_task = loop.create_task(send_page())
                                     send_page_task.add_done_callback(on_page_sent)
 
                         render_task.add_done_callback(handle_children)
                         self._page_futures[render_task.get_name()] = render_task
                 except Exception as err:
                     self._logger.error("Error in page:", err)
+                    if self._on_error is not None:
+                        self._on_error(
+                            IntervalErrorProps(
+                                error=err,
+                                route=inputs.page.slug,
+                                route_definition=self._routes.get(
+                                    inputs.page.slug, None
+                                ),
+                                environment=page_ctx.environment,
+                                user=page_ctx.user,
+                                params=page_ctx.params,
+                                organization=page_ctx.organization,
+                            )
+                        )
                     errors.append(page_error(err, layout_key="children"))
                     page_layout = BasicLayoutModel(kind="BASIC", errors=errors)
 
                     await self._send(
                         "SEND_PAGE",
                         SendPageInputs(
                             page_key=inputs.page_key,
@@ -1292,14 +1425,29 @@
 
             def handle_page_error(task: asyncio.Task):
                 try:
                     task.result()
                 except asyncio.CancelledError:
                     pass
                 except BaseException as err:
+                    self._logger.error(err)
+                    if self._on_error is not None:
+                        self._on_error(
+                            IntervalErrorProps(
+                                error=err,
+                                route=inputs.page.slug,
+                                route_definition=self._routes.get(
+                                    inputs.page.slug, None
+                                ),
+                                environment=page_ctx.environment,
+                                user=page_ctx.user,
+                                params=page_ctx.params,
+                                organization=page_ctx.organization,
+                            )
+                        )
                     errors.append(page_error(err, layout_key="children"))
 
             task = loop.create_task(handle_page(), name="handle_page")
             task.add_done_callback(handle_page_error)
             self._page_futures[inputs.page_key] = task
 
             return OpenPageReturnsSuccess(page_key=inputs.page_key)
```

### Comparing `interval_sdk-1.0.3/src/interval_sdk/superjson/main.py` & `interval_sdk-1.1.0/src/interval_sdk/superjson/main.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/superjson/plainer.py` & `interval_sdk-1.1.0/src/interval_sdk/superjson/plainer.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/superjson/tests/test_superjson.py` & `interval_sdk-1.1.0/src/interval_sdk/superjson/tests/test_superjson.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/superjson/transformer.py` & `interval_sdk-1.1.0/src/interval_sdk/superjson/transformer.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/types.py` & `interval_sdk-1.1.0/src/interval_sdk/types.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/src/interval_sdk/util.py` & `interval_sdk-1.1.0/src/interval_sdk/util.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.3/setup.py` & `interval_sdk-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['aiohttp>=3.8.1,<4.0.0',
  'pydantic>=1.9.0,<2.0.0',
  'typing-extensions>=4.4.0,<5.0.0',
  'websockets>=10.1,<11.0']
 
 setup_kwargs = {
     'name': 'interval-sdk',
-    'version': '1.0.3',
+    'version': '1.1.0',
     'description': "The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more.",
     'long_description': '# interval-sdk\n\n## Installation\n\nInstall using pip, (or your python package manager of choice):\n\n```\npip install interval-sdk\n```\n\n## API\n\n*Note:* Proper documentation is in progress!\n\nSee `src/demos/basic.py` and `src/tests` for a better overview, but in short:\n\n```python\nfrom interval_sdk import Interval, IO\n\n# Initialize Interval\ninterval = Interval("API_KEY")\n\n# Add an action using the function name as the slug\n@interval.action\nasync def hello_interval():\n    return {"hello": "from python!"}\n\n# Add an action using a custom slug (can contain hyphens) and additional configuration\n@interval.action(slug=\'echo-message\', unlisted=True)\nasync def echo_message(io: IO):\n    [message] = await io.group(io.input.text("Hello!", help_text="From python!"))\n\n    return {"message": message}\n\n\n# Synchronously listen, blocking forever\ninterval.listen()\n```\n\nTo not block, interval can also be run asynchronously using\n`interval.listen_async()`. You must provide your own event loop.\n\nThe task will complete as soon as connection to Interval completes, so you\nlikely want to run forever or run alongside another permanent task.\n\n```python\nimport asyncio\n\n# This is what synchronous `listen()` does under the hood\nloop = asyncio.get_event_loop()\ntask = loop.create_task(interval.listen_async())\ndef handle_done(task: asyncio.Task[None]):\n    try:\n        task.result()\n    except:\n        loop.stop()\n\ntask.add_done_callback(handle_done)\nloop.run_forever()\n```\n\nIf you are using `run_forever()`, you\'ll probably want to add signal handlers\nto close the loop gracefully on process termination:\n\n```python\nimport asyncio, signal\n\nloop = asyncio.get_event_loop()\ntask = loop.create_task(interval.listen_async())\ndef handle_done(task: asyncio.Task[None]):\n    try:\n        task.result()\n    except:\n        loop.stop()\n\ntask.add_done_callback(handle_done)\nfor sig in {signal.SIGINT, signal.SIGTERM}:\n    loop.add_signal_handler(sig, loop.stop)\nloop.run_forever()\n```\n\n\n## Contributing\n\nThis project uses [Poetry](https://python-poetry.org/) for dependency\nmanagement\n\n1. `poetry install` to install dependencies\n2. `poetry shell` to activate the virtual environment\n\nTasks are configured using [poethepoet](https://github.com/nat-n/poethepoet)\n(installed as a dev dependency).\n\n- `poe demo [demo_name]` to run a demo (`basic` by default if `demo_name` omitted)\n- `poe test` to run `pytest` (can also run `pytest` directly in virtual env)\n\nCode is formatted using [Black](https://github.com/psf/black). Please configure\nyour editor to format on save using Black, or run `poe format` to format the\ncode before committing changes.\n\n## Tests\n\n*Note:* Tests currently require a local instance of the Interval backend.\n\nTests use [pytest](https://docs.pytest.org/en/7.1.x/) and\n[playwright](https://playwright.dev/python/).\n\nCurrently assumes the `test-runner@interval.com` user exists already.\nRun `yarn test` in the `web` directory at least once to create it before\nrunning these.\n',
     'author': 'Jacob Mischka',
     'author_email': 'jacob@interval.com',
     'maintainer': 'Jacob Mischka',
     'maintainer_email': 'jacob@interval.com',
     'url': 'https://interval.com',
```

### Comparing `interval_sdk-1.0.3/PKG-INFO` & `interval_sdk-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interval-sdk
-Version: 1.0.3
+Version: 1.1.0
 Summary: The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more.
 Home-page: https://interval.com
 Keywords: internal tool,app,ui,ui builder
 Author: Jacob Mischka
 Author-email: jacob@interval.com
 Maintainer: Jacob Mischka
 Maintainer-email: jacob@interval.com
```


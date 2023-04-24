# Comparing `tmp/pool_cue-1.1.1.tar.gz` & `tmp/pool_cue-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pool_cue-1.1.1.tar", max compression
+gzip compressed data, was "pool_cue-1.2.0.tar", max compression
```

## Comparing `pool_cue-1.1.1.tar` & `pool_cue-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1065 2023-04-20 10:20:06.895622 pool_cue-1.1.1/LICENSE
--rw-r--r--   0        0        0     1417 2023-04-20 10:20:06.895622 pool_cue-1.1.1/README.md
--rw-r--r--   0        0        0      309 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/__init__.py
--rw-r--r--   0        0        0      938 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/config.py
--rw-r--r--   0        0        0     1053 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/context.py
--rw-r--r--   0        0        0      158 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/exceptions.py
--rw-r--r--   0        0        0     5709 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/jobs.py
--rw-r--r--   0        0        0     3451 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/queue.py
--rw-r--r--   0        0        0      426 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/serializers.py
--rw-r--r--   0        0        0     2247 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/threading.py
--rw-r--r--   0        0        0      968 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/typing.py
--rw-r--r--   0        0        0     1075 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/utils.py
--rw-r--r--   0        0        0     3967 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pool_cue/worker.py
--rw-r--r--   0        0        0      666 2023-04-20 10:20:06.895622 pool_cue-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 pool_cue-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-24 11:38:38.348888 pool_cue-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1417 2023-04-24 11:38:38.348888 pool_cue-1.2.0/README.md
+-rw-r--r--   0        0        0      309 2023-04-24 11:38:38.348888 pool_cue-1.2.0/pool_cue/__init__.py
+-rw-r--r--   0        0        0      938 2023-04-24 11:38:38.348888 pool_cue-1.2.0/pool_cue/config.py
+-rw-r--r--   0        0        0     1074 2023-04-24 11:38:38.348888 pool_cue-1.2.0/pool_cue/context.py
+-rw-r--r--   0        0        0      158 2023-04-24 11:38:38.348888 pool_cue-1.2.0/pool_cue/exceptions.py
+-rw-r--r--   0        0        0     7083 2023-04-24 11:38:38.348888 pool_cue-1.2.0/pool_cue/jobs.py
+-rw-r--r--   0        0        0     3463 2023-04-24 11:38:38.348888 pool_cue-1.2.0/pool_cue/queue.py
+-rw-r--r--   0        0        0      689 2023-04-24 11:38:38.348888 pool_cue-1.2.0/pool_cue/serializers.py
+-rw-r--r--   0        0        0     2812 2023-04-24 11:38:38.348888 pool_cue-1.2.0/pool_cue/threading.py
+-rw-r--r--   0        0        0      979 2023-04-24 11:38:38.348888 pool_cue-1.2.0/pool_cue/typing.py
+-rw-r--r--   0        0        0     1075 2023-04-24 11:38:38.348888 pool_cue-1.2.0/pool_cue/utils.py
+-rw-r--r--   0        0        0     3966 2023-04-24 11:38:38.348888 pool_cue-1.2.0/pool_cue/worker.py
+-rw-r--r--   0        0        0      666 2023-04-24 11:38:38.348888 pool_cue-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 pool_cue-1.2.0/PKG-INFO
```

### Comparing `pool_cue-1.1.1/LICENSE` & `pool_cue-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pool_cue-1.1.1/README.md` & `pool_cue-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pool_cue-1.1.1/pool_cue/config.py` & `pool_cue-1.2.0/pool_cue/config.py`

 * *Files identical despite different names*

### Comparing `pool_cue-1.1.1/pool_cue/context.py` & `pool_cue-1.2.0/pool_cue/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 __all__ = ["Context", "init_context", "close_context"]
 
 import datetime
 from typing import TypedDict
 from concurrent.futures import ThreadPoolExecutor
 from arq.connections import ArqRedis
 
-from .typing import PushJobFunction
+from .typing import QueueFunction
 from .jobs import push_job
 
 
 class Context(TypedDict):
     redis: ArqRedis
     job_id: str
     job_try: int
     enqueue_time: datetime.datetime
     score: float
 
     # custom
     pool: ThreadPoolExecutor
-    push_job_fn: PushJobFunction
+    queue_fn: QueueFunction
 
 
 async def init_context(ctx: Context, thread_name_prefix: str = "SubThread", max_workers: int | None = None) -> Context:
     """
     Initialize a new thread pool executor in the given worker context.
     """
     ctx["pool"] = ThreadPoolExecutor(thread_name_prefix=thread_name_prefix, max_workers=max_workers)
-    ctx["push_job_fn"] = push_job
+    ctx["queue_fn"] = push_job
     return ctx
 
 
 async def close_context(ctx: Context) -> None:
     """
     Shut down the thread pool executor in the given worker context.
     """
     pool: ThreadPoolExecutor = ctx["pool"]
-    pool.shutdown()
+    pool.shutdown(wait=False, cancel_futures=True)
```

### Comparing `pool_cue-1.1.1/pool_cue/jobs.py` & `pool_cue-1.2.0/pool_cue/jobs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,23 @@
+"""
+Functions used to interact with the queue.
+
+Note: Most of the keyword arguments are prefixed with underscores
+to avoid conflicts with other potential keyword arguments that are passed to the job functions.
+"""
+
 from __future__ import annotations
 
 __all__ = ["get_jobs", "push_job"]
 
 import logging
 import asyncio
 from typing import Callable
 from random import randint
-from arq.jobs import JobDef
+from arq.jobs import JobDef, Job, JobStatus
 from arq.connections import ArqRedis
 
 from .exceptions import QueueError
 from .utils import generate_job_id
 from .typing import GenerateJobIdFunction, AsyncGenerateJobIdFunction
 
 logger: logging.Logger = logging.getLogger(name="pool_cue")
@@ -33,102 +40,133 @@
     except Exception as exc:
         logger.error("Failed to get queued jobs from '%s'!", _queue_name, exc_info=exc)
         raise QueueError("Failed to get queued jobs") from exc
     else:
         return jobs
 
 
-async def _job_already_exists(
-    _redis: ArqRedis, _func: str, _children: list[str] | None = None, _queue_name: str | None = None, **kwargs
-) -> bool:
-    """
-    Check if a job with the given arguments already exists in the queue (queued or running).
-
-    Returns True if:
-
-    - A job with the same function name and keyword arguments (if any) is found.
-    - A job whose function name matches any of the names specified using the '_children' argument is found.
-
-    :param _redis: Redis queue connection.
-    :param _func: Job function name.
-    :param _children: Optional list of other job function names.
-    :param _queue_name: Redis queue name.
-        The default queue name from the Redis connection will be used if not specified.
-    :param kwargs: Optional job function keyword arguments.
-        Used together with the function name to find matching jobs in the queue.
-    :return: Boolean indicating whether the job (or its children) already exists in the queue.
-    """
-    try:
-        jobs: list[JobDef] = await get_jobs(redis=_redis, queue_name=_queue_name)
-    except QueueError as exc:
-        logger.warning("Failed to check if job '%s' already exists in the queue!", _func, exc_info=exc)
-        return True  # return True to keep new jobs from being queued if an error occurs
-    if not _children:
-        return (
-            any(job.function == _func and job.kwargs == kwargs for job in jobs)
-            if kwargs
-            else any(job.function == _func for job in jobs)
-        )
-    return (
-        any((job.function == _func and job.kwargs == kwargs) or job.function in _children for job in jobs)
-        if kwargs
-        else any(job.function == _func or job.function in _children for job in jobs)
-    )
-
-
 async def push_job(
     _redis: ArqRedis,
     _func: str,
     _job_id: str | GenerateJobIdFunction | AsyncGenerateJobIdFunction | None = generate_job_id,
     _children: list[str] | None = None,
     _delay: tuple[int, int] | None = None,
     _force: bool = False,
     _queue_name: str | None = None,
+    *args,
     **kwargs,
 ) -> None:
     """
     Push a new job to the queue.
 
     By default, a job will not be added to the queue if it (or any of its children) already exists in the queue.
-    This behaviour cam be controlled using the '_children' and '_force' keyword arguments.
+    This behaviour can be controlled using the '_job_id', '_children', and '_force' keyword arguments.
 
     :param _redis: Redis queue connection.
     :param _func: Job function name.
     :param _job_id: Optional job ID used by arq to enforce job uniqueness.
         By default, the job will be given an ID based on its function name, children, and keyword arguments.
     :param _children: Optional list of other job function names.
         Used to stop jobs that spawn child jobs from being queued as long as any of its children remain in the queue.
     :param _delay: Duration (in seconds) to wait before running the job.
         The duration will be chosen randomly from within the given range.
     :param _force: If True, the job will be added to the queue even if it or its children already exist in the queue.
         Combine with the '_job_id' argument to skip enforcing job uniqueness.
     :param _queue_name: Redis queue name.
         The default queue name from the Redis connection will be used if not specified.
+    :param args: Positional arguments to pass to the job function.
     :param kwargs: Keyword arguments to pass to the job function.
     """
     _id: str | None
     if isinstance(_job_id, Callable):
         _id = (
             await _job_id(_func=_func, _children=_children, **kwargs)
             if asyncio.iscoroutinefunction(func=_job_id)
             else _job_id(_func=_func, _children=_children, **kwargs)
         )
     else:
         _id = _job_id
     if not _force:
         if await _job_already_exists(
-            _redis=_redis, _func=_func, _children=_children, _queue_name=_queue_name, **kwargs
+            _redis=_redis, _func=_func, _children=_children, _job_id=_id, _queue_name=_queue_name, **kwargs
         ):
             logger.warning("Job '%s' is already queued!", _id or _func)
             return
     _defer_by: int | None = randint(a=_delay[0], b=_delay[1]) if _delay else None
     logger.debug("Adding job '%s' to the queue...", _id or _func)
     try:
         await _redis.enqueue_job(
             function=_func,
             _job_id=_id,
             _queue_name=_queue_name or _redis.default_queue_name,
             _defer_by=_defer_by,
+            *args,
             **kwargs,
         )
     except Exception as exc:
         logger.error("Failed to add job '%s' to the queue!", _id or _func, exc_info=exc)
+
+
+async def _job_already_exists(
+    _redis: ArqRedis,
+    _func: str,
+    _children: list[str] | None = None,
+    _job_id: str | None = None,
+    _queue_name: str | None = None,
+    **kwargs,
+) -> bool:
+    """
+    Check if a job with the given arguments already exists in the queue (queued or running).
+
+    Returns True if:
+
+    - A job with the given job ID is queued or running.
+    - A job with the same function name and keyword arguments (if any) is found.
+    - A job whose function name matches any of the names specified using the '_children' argument is found.
+
+    :param _redis: Redis queue connection.
+    :param _func: Job function name.
+    :param _children: Optional list of other job function names.
+    :param _job_id: Optional job ID.
+    :param _queue_name: Redis queue name.
+        The default queue name from the Redis connection will be used if not specified.
+    :param kwargs: Optional job function keyword arguments.
+        Used together with the function name to find matching jobs in the queue.
+    :return: Boolean indicating whether the job (or its children) already exists in the queue.
+    """
+    if _children or _job_id is None:
+        try:
+            job_defs: list[JobDef] = await get_jobs(redis=_redis, queue_name=_queue_name)
+        except Exception as exc:
+            logger.warning("Failed to check if job '%s' already exists in the queue!", _job_id or _func, exc_info=exc)
+            return True  # return True to keep new jobs from being queued if an error occurs
+        else:
+            return (
+                (
+                    any((j.function == _func and j.kwargs == kwargs) or j.function in _children for j in job_defs)
+                    if kwargs
+                    else any(j.function == _func or j.function in _children for j in job_defs)
+                )
+                if _children
+                else (
+                    any(j.function == _func and j.kwargs == kwargs for j in job_defs)
+                    if kwargs
+                    else any(j.function == _func for j in job_defs)
+                )
+            )
+
+    if _job_id:
+        try:
+            job: Job = Job(
+                job_id=_job_id,
+                redis=_redis,
+                _queue_name=_queue_name or _redis.default_queue_name,
+                _deserializer=_redis.job_deserializer,
+            )
+            status: JobStatus = await job.status()
+        except Exception as exc:
+            logger.warning("Failed to check if job '%s' already exists in the queue!", _job_id, exc_info=exc)
+            return True  # return True to keep new jobs from being queued if an error occurs
+        else:
+            return status in [JobStatus.queued, JobStatus.deferred, JobStatus.in_progress]
+
+    return False
```

### Comparing `pool_cue-1.1.1/pool_cue/queue.py` & `pool_cue-1.2.0/pool_cue/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         _force: bool = False,
         **kwargs,
     ) -> None:
         """
         Push a new job to the queue.
 
         By default, a job will not be added to the queue if it (or any of its children) already exists in the queue.
-        This behaviour cam be controlled using the '_children' and '_force' keyword arguments.
+        This behaviour can be controlled using the '_job_id', '_children', and '_force' keyword arguments.
 
         :param _func: Job function name.
         :param _job_id: Optional job ID used by arq to enforce job uniqueness.
         :param _children: Optional list of other job function names.
             Used to stop new 'parent jobs' from being queued as long as any of its children remain in the queue.
         :param _delay: Duration (in seconds) to wait before running the job.
         :param _force: If True, the job will be added to the queue even if it
```

### Comparing `pool_cue-1.1.1/pool_cue/threading.py` & `pool_cue-1.2.0/pool_cue/threading.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,43 +14,58 @@
 logger: logging.Logger = logging.getLogger(name="pool_cue")
 
 THREAD_POOL_EVENT_LOOPS: dict[int, asyncio.AbstractEventLoop] = {}
 
 
 def _run_coro_in_thread_pool(_coro: Callable, *args, **kwargs) -> None:
     """
-    Function used by 'run_in_thread_pool' to support running asynchronous functions in sub threads:
-    Creates a new event loop in the current (sub) thread (if one doesn't already exist)
+    Function used by 'run_in_thread_pool' to support running asynchronous functions in sub-threads:
+    Creates a new event loop in the current (sub-)thread (if one doesn't already exist)
     to make it possible to call async functions.
 
     Based on:
     https://stackoverflow.com/questions/46074841/why-coroutines-cannot-be-used-with-run-in-executor/63106889#63106889
     """
     current_thread_id: int = threading.current_thread().ident
+    global THREAD_POOL_EVENT_LOOPS
     if current_thread_id not in THREAD_POOL_EVENT_LOOPS:
-        logger.debug("Creating new event loop in sub thread %s...", current_thread_id)
+        logger.debug("Creating new event loop in sub-thread %s...", current_thread_id)
         THREAD_POOL_EVENT_LOOPS[current_thread_id] = asyncio.new_event_loop()
     loop: asyncio.AbstractEventLoop = THREAD_POOL_EVENT_LOOPS[current_thread_id]
     future: Coroutine = _coro(*args, **kwargs)
-    loop.run_until_complete(future=future)
+    try:
+        loop.run_until_complete(future=future)
+    except Exception as exc:
+        logger.warning(
+            "An error occurred while running coroutine '%s' in sub-thread %s!",
+            str(_coro),
+            current_thread_id,
+            exc_info=exc,
+        )
 
 
 async def run_in_thread_pool(_ctx: Context, _func: Callable, *args, **kwargs) -> None:
     """
     Run the given function in the queue worker's dedicated thread pool.
     Use this to run I/O bound tasks without blocking the worker's main thread.
 
     Supports both synchronous and asynchronous functions.
 
     :param _ctx: The worker context.
-    :param _func: The function to run in a sub thread.
+    :param _func: The function to run in a sub-thread.
     :param args: Positional arguments to pass to the function.
     :param kwargs: Keyword arguments to pass to the function.
     """
     loop: asyncio.AbstractEventLoop = asyncio.get_running_loop()
     pool: ThreadPoolExecutor = _ctx["pool"]
     if asyncio.iscoroutinefunction(func=_func):
-        await loop.run_in_executor(
-            executor=pool, func=functools.partial(_run_coro_in_thread_pool, _coro=_func, *args, **kwargs)
-        )
+        try:
+            await loop.run_in_executor(
+                executor=pool, func=functools.partial(_run_coro_in_thread_pool, _coro=_func, *args, **kwargs)
+            )
+        except Exception as exc:
+            logger.warning("Failed to run coroutine in thread pool executor!", exc_info=exc)
     else:
-        await loop.run_in_executor(executor=pool, func=functools.partial(_func, *args, **kwargs))
+        try:
+            await loop.run_in_executor(executor=pool, func=functools.partial(_func, *args, **kwargs))
+        except Exception as exc:
+            logger.warning("Failed to run function in thread pool executor!", exc_info=exc)
```

### Comparing `pool_cue-1.1.1/pool_cue/typing.py` & `pool_cue-1.2.0/pool_cue/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__all__ = ["GenerateJobIdFunction", "AsyncGenerateJobIdFunction", "PushJobFunction"]
+__all__ = ["GenerateJobIdFunction", "AsyncGenerateJobIdFunction", "QueueFunction"]
 
 from typing import Protocol
 from arq.connections import ArqRedis
 
 
 class GenerateJobIdFunction(Protocol):
     __qualname__: str
@@ -16,22 +16,23 @@
 class AsyncGenerateJobIdFunction(Protocol):
     __qualname__: str
 
     async def __call__(self, _func: str, _children: list[str] | None = None, **kwargs) -> str:
         pass
 
 
-class PushJobFunction(Protocol):
+class QueueFunction(Protocol):
     __qualname__: str
 
     async def __call__(
         self,
         _redis: ArqRedis,
         _func: str,
         _job_id: str | GenerateJobIdFunction | AsyncGenerateJobIdFunction | None = None,
         _children: list[str] | None = None,
         _delay: tuple[int, int] | None = None,
         _force: bool = False,
         _queue_name: str | None = None,
+        *args,
         **kwargs,
     ) -> None:
         pass
```

### Comparing `pool_cue-1.1.1/pool_cue/utils.py` & `pool_cue-1.2.0/pool_cue/utils.py`

 * *Files identical despite different names*

### Comparing `pool_cue-1.1.1/pool_cue/worker.py` & `pool_cue-1.2.0/pool_cue/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         on_job_start: StartupShutdown | None = kwargs.get("on_job_start", None)
         on_job_end: StartupShutdown | None = kwargs.get("on_job_end", None)
         after_job_end: StartupShutdown | None = kwargs.get("after_job_end", None)
         handle_signals: bool = kwargs.get("handle_signals", True)
         job_completion_wait: int = kwargs.get("job_completion_wait", 0)
         max_jobs: int = kwargs.get("max_jobs", 20)
         job_timeout: SecondsTimedelta = kwargs.get("job_timeout", 300)
-        keep_result: SecondsTimedelta = kwargs.get("keep_result", 30)
+        keep_result: SecondsTimedelta = kwargs.get("keep_result", 5)
         keep_result_forever: bool = kwargs.get("keep_result_forever", False)
         poll_delay: SecondsTimedelta = kwargs.get("poll_delay", 0.5)
         queue_read_limit: int | None = kwargs.get("queue_read_limit", None)
         max_tries: int = kwargs.get("max_tries", 5)
         health_check_interval: SecondsTimedelta = kwargs.get("health_check_interval", 60)
         health_check_key: str | None = kwargs.get("health_check_key", settings.health_check_key)
         ctx: dict[Any, Any] | None = kwargs.get("ctx", None)
```

### Comparing `pool_cue-1.1.1/pyproject.toml` & `pool_cue-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pool-cue"
-version = "1.1.1"
+version = "1.2.0"
 description = "Tools for working with arq job queues"
 authors = ["skarre-r <skarre-r@protonmail.com>"]
 readme = "README.md"
 repository = "https://github.com/skarre-r/pool-cue"
 packages = [
     { include = "pool_cue" }
 ]
```

### Comparing `pool_cue-1.1.1/PKG-INFO` & `pool_cue-1.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pool-cue
-Version: 1.1.1
+Version: 1.2.0
 Summary: Tools for working with arq job queues
 Home-page: https://github.com/skarre-r/pool-cue
 Author: skarre-r
 Author-email: skarre-r@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```


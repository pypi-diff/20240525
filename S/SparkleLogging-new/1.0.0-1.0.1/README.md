# Comparing `tmp/SparkleLogging-new-1.0.0.tar.gz` & `tmp/SparkleLogging-new-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparkleLogging-new-1.0.0.tar", last modified: Fri May 24 08:49:50 2024, max compression
+gzip compressed data, was "SparkleLogging-new-1.0.1.tar", last modified: Sat May 25 15:27:23 2024, max compression
```

## Comparing `SparkleLogging-new-1.0.0.tar` & `SparkleLogging-new-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 08:49:50.068467 SparkleLogging-new-1.0.0/
--rw-rw-rw-   0        0        0     2973 2024-05-24 08:49:50.066482 SparkleLogging-new-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-24 08:49:49.921823 SparkleLogging-new-1.0.0/SparkleLogging/
--rw-rw-rw-   0        0        0      151 2024-05-21 13:23:09.000000 SparkleLogging-new-1.0.0/SparkleLogging/Interfaces.py
--rw-rw-rw-   0        0        0      246 2024-05-22 10:13:01.000000 SparkleLogging-new-1.0.0/SparkleLogging/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 08:49:49.987646 SparkleLogging-new-1.0.0/SparkleLogging/core/
--rw-rw-rw-   0        0        0        0 2024-05-21 11:03:30.000000 SparkleLogging-new-1.0.0/SparkleLogging/core/__init__.py
--rw-rw-rw-   0        0        0     1370 2024-05-21 15:24:17.000000 SparkleLogging-new-1.0.0/SparkleLogging/core/_excformat.py
--rw-rw-rw-   0        0        0     1270 2024-05-23 11:12:03.000000 SparkleLogging-new-1.0.0/SparkleLogging/core/_formatter.py
--rw-rw-rw-   0        0        0     3712 2024-05-24 08:32:18.000000 SparkleLogging-new-1.0.0/SparkleLogging/core/_handler.py
--rw-rw-rw-   0        0        0      482 2024-05-21 12:04:31.000000 SparkleLogging-new-1.0.0/SparkleLogging/core/_level.py
--rw-rw-rw-   0        0        0     5305 2024-05-24 07:52:20.000000 SparkleLogging-new-1.0.0/SparkleLogging/core/_logger.py
--rw-rw-rw-   0        0        0     1347 2024-05-22 11:34:21.000000 SparkleLogging-new-1.0.0/SparkleLogging/core/_manager.py
--rw-rw-rw-   0        0        0      299 2024-05-24 07:43:55.000000 SparkleLogging-new-1.0.0/SparkleLogging/dependencies.py
-drwxrwxrwx   0        0        0        0 2024-05-24 08:49:49.990640 SparkleLogging-new-1.0.0/SparkleLogging/plugins/
--rw-rw-rw-   0        0        0      450 2024-05-20 15:11:32.000000 SparkleLogging-new-1.0.0/SparkleLogging/plugins/DecoratorsTools.py
--rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 SparkleLogging-new-1.0.0/SparkleLogging/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 08:49:50.009589 SparkleLogging-new-1.0.0/SparkleLogging/utils/
--rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 SparkleLogging-new-1.0.0/SparkleLogging/utils/__init__.py
--rw-rw-rw-   0        0        0      630 2024-05-24 07:35:26.000000 SparkleLogging-new-1.0.0/SparkleLogging/utils/_color.py
--rw-rw-rw-   0        0        0      181 2024-05-21 13:20:01.000000 SparkleLogging-new-1.0.0/SparkleLogging/utils/_types.py
-drwxrwxrwx   0        0        0        0 2024-05-24 08:49:50.065473 SparkleLogging-new-1.0.0/SparkleLogging_new.egg-info/
--rw-rw-rw-   0        0        0     2973 2024-05-24 08:49:48.000000 SparkleLogging-new-1.0.0/SparkleLogging_new.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      660 2024-05-24 08:49:49.000000 SparkleLogging-new-1.0.0/SparkleLogging_new.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 08:49:48.000000 SparkleLogging-new-1.0.0/SparkleLogging_new.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-24 08:49:48.000000 SparkleLogging-new-1.0.0/SparkleLogging_new.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 08:49:50.068467 SparkleLogging-new-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      616 2024-05-24 08:49:45.000000 SparkleLogging-new-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:27:23.233894 SparkleLogging-new-1.0.1/
+-rw-rw-rw-   0        0        0     3453 2024-05-25 15:27:23.231898 SparkleLogging-new-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-25 15:27:23.175949 SparkleLogging-new-1.0.1/SparkleLogging/
+-rw-rw-rw-   0        0        0      151 2024-05-21 13:23:09.000000 SparkleLogging-new-1.0.1/SparkleLogging/Interfaces.py
+-rw-rw-rw-   0        0        0      271 2024-05-25 15:26:21.000000 SparkleLogging-new-1.0.1/SparkleLogging/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:27:23.182929 SparkleLogging-new-1.0.1/SparkleLogging/core/
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:03:30.000000 SparkleLogging-new-1.0.1/SparkleLogging/core/__init__.py
+-rw-rw-rw-   0        0        0     1370 2024-05-21 15:24:17.000000 SparkleLogging-new-1.0.1/SparkleLogging/core/_excformat.py
+-rw-rw-rw-   0        0        0     1270 2024-05-23 11:12:03.000000 SparkleLogging-new-1.0.1/SparkleLogging/core/_formatter.py
+-rw-rw-rw-   0        0        0     3875 2024-05-25 15:08:50.000000 SparkleLogging-new-1.0.1/SparkleLogging/core/_handler.py
+-rw-rw-rw-   0        0        0      493 2024-05-25 14:24:05.000000 SparkleLogging-new-1.0.1/SparkleLogging/core/_level.py
+-rw-rw-rw-   0        0        0     6000 2024-05-25 15:22:52.000000 SparkleLogging-new-1.0.1/SparkleLogging/core/_logger.py
+-rw-rw-rw-   0        0        0     1347 2024-05-24 14:25:39.000000 SparkleLogging-new-1.0.1/SparkleLogging/core/_manager.py
+-rw-rw-rw-   0        0        0      299 2024-05-24 07:43:55.000000 SparkleLogging-new-1.0.1/SparkleLogging/dependencies.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:27:23.183928 SparkleLogging-new-1.0.1/SparkleLogging/plugins/
+-rw-rw-rw-   0        0        0      450 2024-05-20 15:11:32.000000 SparkleLogging-new-1.0.1/SparkleLogging/plugins/DecoratorsTools.py
+-rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 SparkleLogging-new-1.0.1/SparkleLogging/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:27:23.187124 SparkleLogging-new-1.0.1/SparkleLogging/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-20 15:11:32.000000 SparkleLogging-new-1.0.1/SparkleLogging/utils/__init__.py
+-rw-rw-rw-   0        0        0      630 2024-05-24 14:25:14.000000 SparkleLogging-new-1.0.1/SparkleLogging/utils/_color.py
+-rw-rw-rw-   0        0        0      181 2024-05-21 13:20:01.000000 SparkleLogging-new-1.0.1/SparkleLogging/utils/_types.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:27:23.231898 SparkleLogging-new-1.0.1/SparkleLogging_new.egg-info/
+-rw-rw-rw-   0        0        0     3453 2024-05-25 15:27:21.000000 SparkleLogging-new-1.0.1/SparkleLogging_new.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      660 2024-05-25 15:27:21.000000 SparkleLogging-new-1.0.1/SparkleLogging_new.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 15:27:21.000000 SparkleLogging-new-1.0.1/SparkleLogging_new.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-25 15:27:21.000000 SparkleLogging-new-1.0.1/SparkleLogging_new.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 15:27:23.233894 SparkleLogging-new-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      660 2024-05-25 15:26:51.000000 SparkleLogging-new-1.0.1/setup.py
```

### Comparing `SparkleLogging-new-1.0.0/PKG-INFO` & `SparkleLogging-new-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SparkleLogging-new
-Version: 1.0.0
+Version: 1.0.1
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/NewSparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,14 +37,31 @@
 logger.info("test")
 logger.warning("test")
 logger.error("test")
 logger.fatal("test")
 
 ```
 
+# 更新了setLevel接口用于设置日志级别过滤
+
+- 同时修复了一个addNewLevel可能会覆盖自己日志库定义等级的bug
+
+```python
+from SparkleLogging import logger
+from SparkleLogging.core._level import Levels
+
+logger.setLevel(Levels.INFO)
+
+logger.trace("Trace message") # 过滤
+logger.debug("Debug message") # 过滤
+logger.info("Info message")
+logger.warning("Warning message")
+logger.error("Error message")
+logger.fatal("fatal message")
+
 # 添加了addNewLevel方法来提升灵活性
 
 ```python
 from SparkleLogging import logger
 
 TEST = 25
 logger.addNewLevel("test", TEST, 91, "bright_magenta")
```

### Comparing `SparkleLogging-new-1.0.0/SparkleLogging/core/_excformat.py` & `SparkleLogging-new-1.0.1/SparkleLogging/core/_excformat.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-new-1.0.0/SparkleLogging/core/_formatter.py` & `SparkleLogging-new-1.0.1/SparkleLogging/core/_formatter.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-new-1.0.0/SparkleLogging/core/_handler.py` & `SparkleLogging-new-1.0.1/SparkleLogging/core/_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,17 @@
     def __init__(self) -> None:
         self.formatter = None
         self.level = Levels.ON
         self.name = None
         self.log_msg: str = ""
         self.getLevel = _levelToName
 
+    def setLevel(self, level: Level) -> None:
+        self.level = level
+
     def setFormatter(self, formatter: Formatter) -> None:
         self.formatter = formatter
 
     def close(self) -> None:
         pass
 
     def handle(
@@ -44,17 +47,18 @@
         lineno: int,
         funcName: str,
         moduleName: str,
         message: AnyStr,
         level: Level,
         color: str,
     ) -> None:
+        
         if self.formatter is None:
             raise Exception("Formatter not set")
-        
+
         formatted_msg = self.formatter.format(name, threadName,filename,lineno,funcName,moduleName, message, level, color)
         
         return formatted_msg #type: ignore
 
 class StreamHandler(Handler, Writer):
     def __init__(self, error: bool = False) -> None:
         super().__init__()
@@ -92,14 +96,16 @@
                     string = self.queue.get(timeout=1)  # 使用timeout来避免忙等
                     with self.lock:
                         f.write(string + "\n")
                         f.flush()
                     self.queue.task_done()
                 except queue.Empty:
                     pass
+                except Exception as e:
+                    stderr.write(f"{e}\n")
 
     def __del__(self) -> None:
         self.close()
 
     def close(self) -> None:
         self.stop_event.set()
         self.writeThread.join()  # 等待写入线程退出
```

### Comparing `SparkleLogging-new-1.0.0/SparkleLogging/core/_logger.py` & `SparkleLogging-new-1.0.1/SparkleLogging/core/_logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,30 @@
     def close(self) -> None:
         """
         如果只用StreamHandler,则不需要调用此方法,否则必须调用来确保线程被安全关闭
         """
         for handler in self.handlers:
             handler.close()
 
+    def setLevel(self,level:Level):
+        """
+        设置日志等级
+        """
+        if level in _levelToName:
+            with self.lock:
+                if _levelToName[level] == "OFF":
+                    self.level = Levels.OFF
+                else:
+                    if level < Levels.OFF:
+                        self.level = level
+                    else:
+                        raise Exception(f"Level {level} should be less than OFF level")
+        else:
+            raise Exception(f"Level {level} not found")
+
     def addNewLevel(self, name: str, level: Level,colorCode:int,colorName:str) -> None:
         """
         添加自定义等级。
 
         Parameters:
         - name (str): 自定义等级的名称。
         - level (Level): 自定义等级的级别。
@@ -80,14 +96,16 @@
         ```
 
         In this example, a new custom log level named "test" is added with level 25, text color code 91, and color name "bright_magenta".
         """
         # 先判断是否已经有此级别
         if name in self.avaliable_lvl:
             raise Exception(f"Level {name} already exists")
+        elif level in _levelToName:
+            raise Exception(f"your Level value is same as my logging lib`s level: {_levelToName[level]}")
         else:
             with self.lock:
                self.avaliable_lvl[name] = level
                _levelToName[level] = name
                self.colorLevel[level] = colorName #type: ignore
                setattr(_Color, colorName, colorCode)
```

### Comparing `SparkleLogging-new-1.0.0/SparkleLogging/core/_manager.py` & `SparkleLogging-new-1.0.1/SparkleLogging/core/_manager.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-new-1.0.0/SparkleLogging/utils/_color.py` & `SparkleLogging-new-1.0.1/SparkleLogging/utils/_color.py`

 * *Files identical despite different names*

### Comparing `SparkleLogging-new-1.0.0/SparkleLogging_new.egg-info/PKG-INFO` & `SparkleLogging-new-1.0.1/SparkleLogging_new.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SparkleLogging-new
-Version: 1.0.0
+Version: 1.0.1
 Summary: A logging library for Python
 Home-page: https://github.com/KOKOMI12345/NewSparkleLogging
 Author: 花火official
 Author-email: 3072252442@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,14 +37,31 @@
 logger.info("test")
 logger.warning("test")
 logger.error("test")
 logger.fatal("test")
 
 ```
 
+# 更新了setLevel接口用于设置日志级别过滤
+
+- 同时修复了一个addNewLevel可能会覆盖自己日志库定义等级的bug
+
+```python
+from SparkleLogging import logger
+from SparkleLogging.core._level import Levels
+
+logger.setLevel(Levels.INFO)
+
+logger.trace("Trace message") # 过滤
+logger.debug("Debug message") # 过滤
+logger.info("Info message")
+logger.warning("Warning message")
+logger.error("Error message")
+logger.fatal("fatal message")
+
 # 添加了addNewLevel方法来提升灵活性
 
 ```python
 from SparkleLogging import logger
 
 TEST = 25
 logger.addNewLevel("test", TEST, 91, "bright_magenta")
```

### Comparing `SparkleLogging-new-1.0.0/SparkleLogging_new.egg-info/SOURCES.txt` & `SparkleLogging-new-1.0.1/SparkleLogging_new.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SparkleLogging-new-1.0.0/setup.py` & `SparkleLogging-new-1.0.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup, find_packages
+from SparkleLogging import __version__
 
 setup(
     name='SparkleLogging-new',
-    version='1.0.0',
+    version=__version__,
     packages=find_packages(),
     author='花火official',
     author_email='3072252442@qq.com',
     description='A logging library for Python',
     long_description=open('Readme.md','r',encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KOKOMI12345/NewSparkleLogging',
```


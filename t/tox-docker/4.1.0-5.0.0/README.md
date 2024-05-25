# Comparing `tmp/tox-docker-4.1.0.tar.gz` & `tmp/tox_docker-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tox-docker-4.1.0.tar", last modified: Sun Mar 26 12:33:51 2023, max compression
+gzip compressed data, was "tox_docker-5.0.0.tar", last modified: Sat May 25 12:46:01 2024, max compression
```

## Comparing `tox-docker-4.1.0.tar` & `tox_docker-5.0.0.tar`

### file list

```diff
@@ -1,42 +1,31 @@
-drwxr-xr-x   0 dcrosta    (501) staff       (20)        0 2023-03-26 12:33:51.182656 tox-docker-4.1.0/
--rw-r--r--   0 dcrosta    (501) staff       (20)     1490 2019-06-17 23:23:12.000000 tox-docker-4.1.0/LICENSE
--rw-r--r--   0 dcrosta    (501) staff       (20)      147 2020-06-08 19:00:53.000000 tox-docker-4.1.0/MANIFEST.in
--rw-r--r--   0 dcrosta    (501) staff       (20)    11867 2023-03-26 12:33:51.182725 tox-docker-4.1.0/PKG-INFO
--rw-r--r--   0 dcrosta    (501) staff       (20)    11156 2023-03-26 12:09:50.000000 tox-docker-4.1.0/README.rst
--rw-r--r--   0 dcrosta    (501) staff       (20)      101 2020-07-31 12:43:42.000000 tox-docker-4.1.0/pyproject.toml
--rw-r--r--   0 dcrosta    (501) staff       (20)      409 2023-03-26 12:33:51.183088 tox-docker-4.1.0/setup.cfg
--rw-r--r--   0 dcrosta    (501) staff       (20)     1006 2023-03-21 13:36:09.000000 tox-docker-4.1.0/setup.py
-drwxr-xr-x   0 dcrosta    (501) staff       (20)        0 2023-03-26 12:33:51.179520 tox-docker-4.1.0/tox_docker/
--rw-r--r--   0 dcrosta    (501) staff       (20)      360 2022-01-22 14:23:00.000000 tox-docker-4.1.0/tox_docker/__init__.py
--rw-r--r--   0 dcrosta    (501) staff       (20)     5420 2023-03-26 12:09:50.000000 tox-docker-4.1.0/tox_docker/config.py
--rw-r--r--   0 dcrosta    (501) staff       (20)       61 2022-01-22 14:23:00.000000 tox-docker-4.1.0/tox_docker/log.py
--rw-r--r--   0 dcrosta    (501) staff       (20)     7534 2023-03-26 12:09:50.000000 tox-docker-4.1.0/tox_docker/plugin.py
-drwxr-xr-x   0 dcrosta    (501) staff       (20)        0 2023-03-26 12:33:51.181723 tox-docker-4.1.0/tox_docker/tests/
--rw-r--r--   0 dcrosta    (501) staff       (20)        0 2020-06-08 19:00:53.000000 tox-docker-4.1.0/tox_docker/tests/__init__.py
--rw-r--r--   0 dcrosta    (501) staff       (20)      674 2023-03-26 12:09:50.000000 tox-docker-4.1.0/tox_docker/tests/test_containers.py
--rw-r--r--   0 dcrosta    (501) staff       (20)      656 2022-01-22 14:23:00.000000 tox-docker-4.1.0/tox_docker/tests/test_env_vars.py
--rw-r--r--   0 dcrosta    (501) staff       (20)     1569 2022-01-22 14:23:00.000000 tox-docker-4.1.0/tox_docker/tests/test_gateway.py
--rw-r--r--   0 dcrosta    (501) staff       (20)      439 2022-01-22 14:23:00.000000 tox-docker-4.1.0/tox_docker/tests/test_healthcheck.py
--rw-r--r--   0 dcrosta    (501) staff       (20)      916 2022-01-22 14:23:00.000000 tox-docker-4.1.0/tox_docker/tests/test_images.py
--rw-r--r--   0 dcrosta    (501) staff       (20)      793 2022-01-22 14:23:00.000000 tox-docker-4.1.0/tox_docker/tests/test_links.py
--rw-r--r--   0 dcrosta    (501) staff       (20)      839 2023-02-14 12:36:37.000000 tox-docker-4.1.0/tox_docker/tests/test_ports.py
--rw-r--r--   0 dcrosta    (501) staff       (20)      330 2022-01-22 14:23:00.000000 tox-docker-4.1.0/tox_docker/tests/test_volumes.py
--rw-r--r--   0 dcrosta    (501) staff       (20)      753 2022-01-22 14:23:00.000000 tox-docker-4.1.0/tox_docker/tests/util.py
-drwxr-xr-x   0 dcrosta    (501) staff       (20)        0 2023-03-26 12:33:51.182156 tox-docker-4.1.0/tox_docker/tox3/
--rw-r--r--   0 dcrosta    (501) staff       (20)        0 2022-01-22 14:23:00.000000 tox-docker-4.1.0/tox_docker/tox3/__init__.py
--rw-r--r--   0 dcrosta    (501) staff       (20)     4871 2023-03-26 12:09:50.000000 tox-docker-4.1.0/tox_docker/tox3/config.py
--rw-r--r--   0 dcrosta    (501) staff       (20)      427 2022-01-22 14:23:00.000000 tox-docker-4.1.0/tox_docker/tox3/log.py
--rw-r--r--   0 dcrosta    (501) staff       (20)     4548 2023-03-26 12:09:50.000000 tox-docker-4.1.0/tox_docker/tox3/plugin.py
-drwxr-xr-x   0 dcrosta    (501) staff       (20)        0 2023-03-26 12:33:51.182559 tox-docker-4.1.0/tox_docker/tox4/
--rw-r--r--   0 dcrosta    (501) staff       (20)        0 2022-01-22 14:23:00.000000 tox-docker-4.1.0/tox_docker/tox4/__init__.py
--rw-r--r--   0 dcrosta    (501) staff       (20)     4274 2023-03-26 12:09:50.000000 tox-docker-4.1.0/tox_docker/tox4/config.py
--rw-r--r--   0 dcrosta    (501) staff       (20)      103 2022-01-22 14:23:00.000000 tox-docker-4.1.0/tox_docker/tox4/log.py
--rw-r--r--   0 dcrosta    (501) staff       (20)     3941 2023-03-26 12:09:50.000000 tox-docker-4.1.0/tox_docker/tox4/plugin.py
-drwxr-xr-x   0 dcrosta    (501) staff       (20)        0 2023-03-26 12:33:51.180119 tox-docker-4.1.0/tox_docker.egg-info/
--rw-r--r--   0 dcrosta    (501) staff       (20)    11867 2023-03-26 12:33:51.000000 tox-docker-4.1.0/tox_docker.egg-info/PKG-INFO
--rw-r--r--   0 dcrosta    (501) staff       (20)      892 2023-03-26 12:33:51.000000 tox-docker-4.1.0/tox_docker.egg-info/SOURCES.txt
--rw-r--r--   0 dcrosta    (501) staff       (20)        1 2023-03-26 12:33:51.000000 tox-docker-4.1.0/tox_docker.egg-info/dependency_links.txt
--rw-r--r--   0 dcrosta    (501) staff       (20)       27 2023-03-26 12:33:51.000000 tox-docker-4.1.0/tox_docker.egg-info/entry_points.txt
--rw-r--r--   0 dcrosta    (501) staff       (20)       43 2023-03-26 12:33:51.000000 tox-docker-4.1.0/tox_docker.egg-info/requires.txt
--rw-r--r--   0 dcrosta    (501) staff       (20)       11 2023-03-26 12:33:51.000000 tox-docker-4.1.0/tox_docker.egg-info/top_level.txt
--rw-r--r--   0 dcrosta    (501) staff       (20)       17 2023-03-26 12:33:51.000000 tox-docker-4.1.0/version.txt
+drwxr-xr-x   0 dcrosta    (501) staff       (20)        0 2024-05-25 12:46:01.946532 tox_docker-5.0.0/
+-rw-r--r--   0 dcrosta    (501) staff       (20)     1490 2019-06-17 23:23:12.000000 tox_docker-5.0.0/LICENSE
+-rw-r--r--   0 dcrosta    (501) staff       (20)      147 2020-06-08 19:00:53.000000 tox_docker-5.0.0/MANIFEST.in
+-rw-r--r--   0 dcrosta    (501) staff       (20)    11983 2024-05-25 12:46:01.946427 tox_docker-5.0.0/PKG-INFO
+-rw-r--r--   0 dcrosta    (501) staff       (20)    11228 2024-05-25 12:43:51.000000 tox_docker-5.0.0/README.rst
+-rw-r--r--   0 dcrosta    (501) staff       (20)      101 2020-07-31 12:43:42.000000 tox_docker-5.0.0/pyproject.toml
+-rw-r--r--   0 dcrosta    (501) staff       (20)      396 2024-05-25 12:46:01.946760 tox_docker-5.0.0/setup.cfg
+-rw-r--r--   0 dcrosta    (501) staff       (20)     1003 2024-05-25 12:38:18.000000 tox_docker-5.0.0/setup.py
+drwxr-xr-x   0 dcrosta    (501) staff       (20)        0 2024-05-25 12:46:01.944134 tox_docker-5.0.0/tox_docker/
+-rw-r--r--   0 dcrosta    (501) staff       (20)       32 2023-07-13 20:28:38.000000 tox_docker-5.0.0/tox_docker/__init__.py
+-rw-r--r--   0 dcrosta    (501) staff       (20)    10507 2024-05-25 12:38:18.000000 tox_docker-5.0.0/tox_docker/config.py
+-rw-r--r--   0 dcrosta    (501) staff       (20)    11562 2023-07-20 17:26:38.000000 tox_docker-5.0.0/tox_docker/plugin.py
+drwxr-xr-x   0 dcrosta    (501) staff       (20)        0 2024-05-25 12:46:01.946061 tox_docker-5.0.0/tox_docker/tests/
+-rw-r--r--   0 dcrosta    (501) staff       (20)        0 2020-06-08 19:00:53.000000 tox_docker-5.0.0/tox_docker/tests/__init__.py
+-rw-r--r--   0 dcrosta    (501) staff       (20)      674 2023-03-26 12:09:50.000000 tox_docker-5.0.0/tox_docker/tests/test_containers.py
+-rw-r--r--   0 dcrosta    (501) staff       (20)      785 2023-07-20 17:26:38.000000 tox_docker-5.0.0/tox_docker/tests/test_env_vars.py
+-rw-r--r--   0 dcrosta    (501) staff       (20)     1569 2022-01-22 14:23:00.000000 tox_docker-5.0.0/tox_docker/tests/test_gateway.py
+-rw-r--r--   0 dcrosta    (501) staff       (20)      439 2022-01-22 14:23:00.000000 tox_docker-5.0.0/tox_docker/tests/test_healthcheck.py
+-rw-r--r--   0 dcrosta    (501) staff       (20)      916 2022-01-22 14:23:00.000000 tox_docker-5.0.0/tox_docker/tests/test_images.py
+-rw-r--r--   0 dcrosta    (501) staff       (20)      793 2022-01-22 14:23:00.000000 tox_docker-5.0.0/tox_docker/tests/test_links.py
+-rw-r--r--   0 dcrosta    (501) staff       (20)     1257 2023-07-20 17:26:38.000000 tox_docker-5.0.0/tox_docker/tests/test_ports.py
+-rw-r--r--   0 dcrosta    (501) staff       (20)      330 2022-01-22 14:23:00.000000 tox_docker-5.0.0/tox_docker/tests/test_volumes.py
+-rw-r--r--   0 dcrosta    (501) staff       (20)      753 2022-01-22 14:23:00.000000 tox_docker-5.0.0/tox_docker/tests/util.py
+drwxr-xr-x   0 dcrosta    (501) staff       (20)        0 2024-05-25 12:46:01.946224 tox_docker-5.0.0/tox_docker.egg-info/
+-rw-r--r--   0 dcrosta    (501) staff       (20)    11983 2024-05-25 12:46:01.000000 tox_docker-5.0.0/tox_docker.egg-info/PKG-INFO
+-rw-r--r--   0 dcrosta    (501) staff       (20)      668 2024-05-25 12:46:01.000000 tox_docker-5.0.0/tox_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 dcrosta    (501) staff       (20)        1 2024-05-25 12:46:01.000000 tox_docker-5.0.0/tox_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 dcrosta    (501) staff       (20)       26 2024-05-25 12:46:01.000000 tox_docker-5.0.0/tox_docker.egg-info/entry_points.txt
+-rw-r--r--   0 dcrosta    (501) staff       (20)       33 2024-05-25 12:46:01.000000 tox_docker-5.0.0/tox_docker.egg-info/requires.txt
+-rw-r--r--   0 dcrosta    (501) staff       (20)       11 2024-05-25 12:46:01.000000 tox_docker-5.0.0/tox_docker.egg-info/top_level.txt
+-rw-r--r--   0 dcrosta    (501) staff       (20)       17 2024-05-25 12:46:01.000000 tox_docker-5.0.0/version.txt
```

### Comparing `tox-docker-4.1.0/LICENSE` & `tox_docker-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-docker-4.1.0/PKG-INFO` & `tox_docker-5.0.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: tox-docker
-Version: 4.1.0
-Summary: Launch a docker instance around test runs
-Home-page: https://github.com/tox-dev/tox-docker
-Maintainer: Dan Crosta
-Maintainer-email: dcrosta@late.am
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Plugins
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Testing
-License-File: LICENSE
-
 ============
  tox-docker
 ============
 
 A `tox <https://tox.readthedocs.io/en/latest/>`__ plugin which runs one or
 more `Docker <https://www.docker.com/>`__ containers during the test run.
 
@@ -89,45 +69,35 @@
     is raised if ``dockerfile_target`` is set without ``dockerfile`` set.
 
 ``environment``
     A multi-line list of ``KEY=value`` settings which is used to set
     environment variables for the container. The variables are only available
     to the container, not to other containers or the test environment.
 
-``ports``
+``expose``
     A multi-line list of port mapping specifications, as
-    ``HOST_PORT:CONTAINER_PORT/PROTO``, which causes the container's
-    ``EXPOSE`` d port to be available on ``HOST_PORT``. See below for
-    more on port mapping.
-
-    If ``ports`` is not specified, all the container's ``EXPOSE`` d ports are
-    mapped (equivalent to ``docker run -P ...``)
-
-    For each mapped port, an environment variable of the form
-    ``<container-name>_<port-number>_<protocol>_PORT`` (eg
-    ``NGINX_80_TCP_PORT`` or ``TELEGRAF_8092_UDP_PORT``) is set for the test
-    run.
-
-    For each container, an environment variable of the form
-    ``<container_name>_HOST`` is set for the test run, indicating the host
-    name or IP address to use to communicate with the container.
-
-    If you set the ``HOST_PORT`` to zero, a random available port will be
-    assigned on the tox host. This is useful in case the container does not
-    ``EXPOSE`` the port you need, or if you want to map only some of the
-    ``EXPOSE``\d ports.
-
-    In both environment variables, the container name part is converted to
-    upper case, and all non-alphanumeric characters are replaced with an
+    ``ENV_VAR=CONTAINER_PORT/PROTO``. Within the testenv, the environment
+    variable ``ENV_VAR`` will contain the port number to connect to the
+    docker container's ``EXPOSE`` d port. If ``expose`` is specified, only
+    the listed ports will have environment variables created for them.
+
+    If ``expose`` is not specified, all the container's ``EXPOSE`` d ports
+    are made available (equivalent to ``docker run -P ...``) using default
+    environment variable names of the form
+    ``<container-name>_<port-number>_<protocol>_PORT`` (eg ``NGINX_80_TCP_PORT``
+    or ``TELEGRAF_8092_UDP_PORT``), with the container name and protocol
+    converted to upper case, and non-alphanumeric characters replaced with an
     underscore (``_``).
 
-    Tox-docker does not attempt to ensure that you have proper permission to
-    bind the ``HOST_PORT``, that it is not already bound and listening, etc;
-    if you explicitly list ports, it is your responsibility to ensure that
-    it can be successfully mapped.
+``host_var``
+    The name of an environment variable that will contain the hostname or IP
+    address to use to communicate with the container. Defaults to
+    ``<container_name>_HOST`` if not set, with the container name converted to
+    upper case, and non-alphanumeric characters replaced with an underscore
+    (``_``).
 
 ``links``
     A multi-line list of `container links
     <https://docs.docker.com/network/links/>`__, as ``other-container-name``
     or ``other-container-name:alias``. If no alias is given, the
     ``other-container-name`` is used. Within the container, the ``EXPOSE`` d
     ports of the other container will be available via the alias as hostname.
@@ -146,15 +116,15 @@
     and ``inside_path`` must be absolute paths.
 
 ``healthcheck_cmd``, ``healthcheck_interval``, ``healthcheck_retries``, ``healthcheck_start_period``, ``healthcheck_timeout``
     These set or customize parameters of the container `health check
     <https://docs.docker.com/engine/reference/builder/#healthcheck>`__. The
     ``healthcheck_interval``, ``healthcheck_start_period``, and
     ``healthcheck_timeout`` are specified as a number of seconds.
-    The ``healtcheck_cmd`` is an argv list which must name a command and
+    ``healthcheck_cmd`` is an argv list which must name a command and
     arguments that can be run within the container; if not specified, any
     health check built in to the container is used.
 
     If any healthcheck parameters are defined, tox-docker will delay the
     test run until the container reports healthy, and will fail the test
     run if it never does so (within the parameters specified).
 
@@ -222,40 +192,57 @@
 
     [docker:appserv]
     # You can use any value that `docker run` would accept as the image
     image = your-registry.example.org:1234/your-appserv
     # Within the appserv container, host "db" is linked to the postgres container
     links =
         db:db
-    # Use ports to expose specific ports; if you don't specify ports, then all
-    # the EXPOSEd ports defined by the image are mapped to an available
-    # ephemeral port.
-    ports =
-        8080:8080/tcp
+    # Expose ports to the testenv
+    expose =
+        APP_HTTP_PORT=8080/tcp
 
 
 Environment Variables
 ---------------------
 
 If you are running in a Docker-In-Docker environment, you can override the address
 used for port checking using the environment variable ``TOX_DOCKER_GATEWAY``. This
 variable should be the hostname or ip address used to connect to the container.
 
 Version Compatibility
 ---------------------
 
-Tox-docker requires tox to be run in Python 3.7 or newer, and requires tox
-version 3.0 or newer. Older versions of tox-docker may work with older
+Tox-docker requires tox to be run in Python 3.8 or newer, and requires tox
+version 4 or newer. Older versions of tox-docker may work with older
 versions of Python or tox, but these configurations are no longer supported.
 
+Upgrading
+---------
+
+Some configuration options were removed:
+
+New in 5.0:
+
+``ports``
+    This directive was removed in tox-docker version 5.0. Use ``expose``
+    instead. The ability to map a container port to a specific host port was
+    completely removed.
+
 
 ==========
 Change Log
 ==========
 
+* 5.0.0
+    * Remove support for tox 3
+    * Removed support for Python 3.7 and earlier
+    * Remove ``ports``; add ``expose`` and ``host_var``
+    * Support ``docker`` (the Python module) 7.x (thanks @jonathangreen)
+* 4.1.1
+    * Fix typo in README (thanks @akx)
 * 4.1.0
     * Drop test support for docker (Python library) 3.x; add test support
       for docker 6.x. Other versions may work, but we only support tested
       versions.
     * Add support for ``dockerfile`` and ``dockerfile_target`` directives
       to build local images
 * 4.0.0
@@ -282,17 +269,15 @@
 Development
 ===========
 
 Code Style
 ----------
 
 Tox-docker uses black and isort to enforce style standards on the codebase.
-The formatting is orindaily done for you via `pre-commit
+The formatting is ordinarily done for you via `pre-commit
 <https://pre-commit.com/>`_, and is enforced via the ``tox -e style`` build.
 To work on tox-docker locally with pre-commit, `pip install -r
 dev-requirements.txt`` and ``pre-commit install`` to set up the git hooks;
 subsequently, when you ``git commit``, the formatter will be run. If the
 changed files are not conformant, the hook will have reformatted them and
 you may need to run pre-commit again. You can run ``pre-commit run --files
 *.py`` to manually run the formatters.
-
-
```

### Comparing `tox-docker-4.1.0/README.rst` & `tox_docker-5.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: tox-docker
+Version: 5.0.0
+Summary: Manage lifecycle of docker containers during Tox test runs
+Home-page: https://github.com/tox-dev/tox-docker
+Maintainer: Dan Crosta
+Maintainer-email: dcrosta@late.am
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Plugins
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Testing
+License-File: LICENSE
+Requires-Dist: docker<8.0,>=4.0
+Requires-Dist: tox<5.0,>=4.0.0
+
 ============
  tox-docker
 ============
 
 A `tox <https://tox.readthedocs.io/en/latest/>`__ plugin which runs one or
 more `Docker <https://www.docker.com/>`__ containers during the test run.
 
@@ -69,45 +89,35 @@
     is raised if ``dockerfile_target`` is set without ``dockerfile`` set.
 
 ``environment``
     A multi-line list of ``KEY=value`` settings which is used to set
     environment variables for the container. The variables are only available
     to the container, not to other containers or the test environment.
 
-``ports``
+``expose``
     A multi-line list of port mapping specifications, as
-    ``HOST_PORT:CONTAINER_PORT/PROTO``, which causes the container's
-    ``EXPOSE`` d port to be available on ``HOST_PORT``. See below for
-    more on port mapping.
-
-    If ``ports`` is not specified, all the container's ``EXPOSE`` d ports are
-    mapped (equivalent to ``docker run -P ...``)
-
-    For each mapped port, an environment variable of the form
-    ``<container-name>_<port-number>_<protocol>_PORT`` (eg
-    ``NGINX_80_TCP_PORT`` or ``TELEGRAF_8092_UDP_PORT``) is set for the test
-    run.
-
-    For each container, an environment variable of the form
-    ``<container_name>_HOST`` is set for the test run, indicating the host
-    name or IP address to use to communicate with the container.
-
-    If you set the ``HOST_PORT`` to zero, a random available port will be
-    assigned on the tox host. This is useful in case the container does not
-    ``EXPOSE`` the port you need, or if you want to map only some of the
-    ``EXPOSE``\d ports.
-
-    In both environment variables, the container name part is converted to
-    upper case, and all non-alphanumeric characters are replaced with an
+    ``ENV_VAR=CONTAINER_PORT/PROTO``. Within the testenv, the environment
+    variable ``ENV_VAR`` will contain the port number to connect to the
+    docker container's ``EXPOSE`` d port. If ``expose`` is specified, only
+    the listed ports will have environment variables created for them.
+
+    If ``expose`` is not specified, all the container's ``EXPOSE`` d ports
+    are made available (equivalent to ``docker run -P ...``) using default
+    environment variable names of the form
+    ``<container-name>_<port-number>_<protocol>_PORT`` (eg ``NGINX_80_TCP_PORT``
+    or ``TELEGRAF_8092_UDP_PORT``), with the container name and protocol
+    converted to upper case, and non-alphanumeric characters replaced with an
     underscore (``_``).
 
-    Tox-docker does not attempt to ensure that you have proper permission to
-    bind the ``HOST_PORT``, that it is not already bound and listening, etc;
-    if you explicitly list ports, it is your responsibility to ensure that
-    it can be successfully mapped.
+``host_var``
+    The name of an environment variable that will contain the hostname or IP
+    address to use to communicate with the container. Defaults to
+    ``<container_name>_HOST`` if not set, with the container name converted to
+    upper case, and non-alphanumeric characters replaced with an underscore
+    (``_``).
 
 ``links``
     A multi-line list of `container links
     <https://docs.docker.com/network/links/>`__, as ``other-container-name``
     or ``other-container-name:alias``. If no alias is given, the
     ``other-container-name`` is used. Within the container, the ``EXPOSE`` d
     ports of the other container will be available via the alias as hostname.
@@ -126,15 +136,15 @@
     and ``inside_path`` must be absolute paths.
 
 ``healthcheck_cmd``, ``healthcheck_interval``, ``healthcheck_retries``, ``healthcheck_start_period``, ``healthcheck_timeout``
     These set or customize parameters of the container `health check
     <https://docs.docker.com/engine/reference/builder/#healthcheck>`__. The
     ``healthcheck_interval``, ``healthcheck_start_period``, and
     ``healthcheck_timeout`` are specified as a number of seconds.
-    The ``healtcheck_cmd`` is an argv list which must name a command and
+    ``healthcheck_cmd`` is an argv list which must name a command and
     arguments that can be run within the container; if not specified, any
     health check built in to the container is used.
 
     If any healthcheck parameters are defined, tox-docker will delay the
     test run until the container reports healthy, and will fail the test
     run if it never does so (within the parameters specified).
 
@@ -202,40 +212,57 @@
 
     [docker:appserv]
     # You can use any value that `docker run` would accept as the image
     image = your-registry.example.org:1234/your-appserv
     # Within the appserv container, host "db" is linked to the postgres container
     links =
         db:db
-    # Use ports to expose specific ports; if you don't specify ports, then all
-    # the EXPOSEd ports defined by the image are mapped to an available
-    # ephemeral port.
-    ports =
-        8080:8080/tcp
+    # Expose ports to the testenv
+    expose =
+        APP_HTTP_PORT=8080/tcp
 
 
 Environment Variables
 ---------------------
 
 If you are running in a Docker-In-Docker environment, you can override the address
 used for port checking using the environment variable ``TOX_DOCKER_GATEWAY``. This
 variable should be the hostname or ip address used to connect to the container.
 
 Version Compatibility
 ---------------------
 
-Tox-docker requires tox to be run in Python 3.7 or newer, and requires tox
-version 3.0 or newer. Older versions of tox-docker may work with older
+Tox-docker requires tox to be run in Python 3.8 or newer, and requires tox
+version 4 or newer. Older versions of tox-docker may work with older
 versions of Python or tox, but these configurations are no longer supported.
 
+Upgrading
+---------
+
+Some configuration options were removed:
+
+New in 5.0:
+
+``ports``
+    This directive was removed in tox-docker version 5.0. Use ``expose``
+    instead. The ability to map a container port to a specific host port was
+    completely removed.
+
 
 ==========
 Change Log
 ==========
 
+* 5.0.0
+    * Remove support for tox 3
+    * Removed support for Python 3.7 and earlier
+    * Remove ``ports``; add ``expose`` and ``host_var``
+    * Support ``docker`` (the Python module) 7.x (thanks @jonathangreen)
+* 4.1.1
+    * Fix typo in README (thanks @akx)
 * 4.1.0
     * Drop test support for docker (Python library) 3.x; add test support
       for docker 6.x. Other versions may work, but we only support tested
       versions.
     * Add support for ``dockerfile`` and ``dockerfile_target`` directives
       to build local images
 * 4.0.0
@@ -262,15 +289,15 @@
 Development
 ===========
 
 Code Style
 ----------
 
 Tox-docker uses black and isort to enforce style standards on the codebase.
-The formatting is orindaily done for you via `pre-commit
+The formatting is ordinarily done for you via `pre-commit
 <https://pre-commit.com/>`_, and is enforced via the ``tox -e style`` build.
 To work on tox-docker locally with pre-commit, `pip install -r
 dev-requirements.txt`` and ``pre-commit install`` to set up the git hooks;
 subsequently, when you ``git commit``, the formatter will be run. If the
 changed files are not conformant, the hook will have reformatted them and
 you may need to run pre-commit again. You can run ``pre-commit run --files
 *.py`` to manually run the formatters.
```

### Comparing `tox-docker-4.1.0/setup.py` & `tox_docker-5.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from setuptools import find_packages, setup
 
 setup(
     name="tox-docker",
-    description="Launch a docker instance around test runs",
+    description="Manage lifecycle of docker containers during Tox test runs",
     long_description=open("README.rst").read(),
     url="https://github.com/tox-dev/tox-docker",
     maintainer="Dan Crosta",
     maintainer_email="dcrosta@late.am",
     install_requires=[
-        "docker>=4.0,<7.0",
-        "packaging",
-        "tox>=3.0.0,<5.0",
+        "docker>=4.0,<8.0",
+        "tox>=4.0.0,<5.0",
     ],
     packages=find_packages(),
     entry_points={"tox": ["docker = tox_docker"]},
     vcversioner={"version_module_paths": ["_version.py"]},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Plugins",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Testing",
     ],
 )
```

### Comparing `tox-docker-4.1.0/tox_docker/tests/test_containers.py` & `tox_docker-5.0.0/tox_docker/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `tox-docker-4.1.0/tox_docker/tests/test_gateway.py` & `tox_docker-5.0.0/tox_docker/tests/test_gateway.py`

 * *Files identical despite different names*

### Comparing `tox-docker-4.1.0/tox_docker/tests/test_images.py` & `tox_docker-5.0.0/tox_docker/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `tox-docker-4.1.0/tox_docker/tests/test_links.py` & `tox_docker-5.0.0/tox_docker/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `tox-docker-4.1.0/tox_docker/tests/test_ports.py` & `tox_docker-5.0.0/tox_docker/tests/test_ports.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,36 @@
 from urllib.request import urlopen
 import os
 
 
+def test_default_host_name_var() -> None:
+    # [docker:healthcheck-builtin] doesn't specify host_var
+    assert "HEALTHCHECK_BUILTIN_HOST" in os.environ
+
+
+def test_custom_host_name_var() -> None:
+    # [docker:healthcheck-custom] _does_ specify host_var=...
+    assert "NET_TWO_CUSTOM_HOST" in os.environ
+
+
+def test_EXPOSEd_ports_are_available_when_expose_is_not_set() -> None:
+    # [docker:healthcheck-builtin] does not have expose=
+    assert "HEALTHCHECK_BUILTIN_8000_TCP_PORT" in os.environ
+
+
+def test_EXPOSEd_ports_are_not_available_if_not_listed_in_expose() -> None:
+    # [docker:networking-two] doesn't map 5678/udp, but it is EXPOSEd
+    assert "NETWORKING_TWO_5678_UDP_PORT" not in os.environ
+
+
+def test_manually_mapped_ports_dont_get_default_port_envvar() -> None:
+    # [docker:networking-two] explicitly maps 1234/tcp
+    assert "NETWORKING_TWO_1234_TCP_PORT" not in os.environ
+
+
 def test_exposed_ports_are_accessible_to_test_runs() -> None:
     host = os.environ["HEALTHCHECK_BUILTIN_HOST"]
     port = os.environ["HEALTHCHECK_BUILTIN_8000_TCP_PORT"]
 
     response = urlopen(f"http://{host}:{port}/")
     assert response.getcode() == 200
     assert b"Directory listing for /" in response.read()
-
-
-def test_it_exposes_only_specified_port() -> None:
-    # this container remaps 1234/tcp to 2345, and hides 5678/udp
-    assert os.environ["NETWORKING_TWO_1234_TCP_PORT"] == "2345"
-    assert "NETWORKING_TWO_5678_UDP_PORT" not in os.environ
-
-
-def test_docker_picks_a_port_when_you_map_to_zero() -> None:
-    # tox.ini has `ports = 0:1234/tcp 0:5678/udp`
-    assert os.environ["NETWORKING_ONE_1234_TCP_PORT"] != "0"
-    assert os.environ["NETWORKING_ONE_5678_UDP_PORT"] != "0"
```

### Comparing `tox-docker-4.1.0/tox_docker/tests/util.py` & `tox_docker-5.0.0/tox_docker/tests/util.py`

 * *Files identical despite different names*

### Comparing `tox-docker-4.1.0/tox_docker.egg-info/PKG-INFO` & `tox_docker-5.0.0/tox_docker.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: tox-docker
-Version: 4.1.0
-Summary: Launch a docker instance around test runs
+Version: 5.0.0
+Summary: Manage lifecycle of docker containers during Tox test runs
 Home-page: https://github.com/tox-dev/tox-docker
 Maintainer: Dan Crosta
 Maintainer-email: dcrosta@late.am
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 License-File: LICENSE
+Requires-Dist: docker<8.0,>=4.0
+Requires-Dist: tox<5.0,>=4.0.0
 
 ============
  tox-docker
 ============
 
 A `tox <https://tox.readthedocs.io/en/latest/>`__ plugin which runs one or
 more `Docker <https://www.docker.com/>`__ containers during the test run.
@@ -89,45 +89,35 @@
     is raised if ``dockerfile_target`` is set without ``dockerfile`` set.
 
 ``environment``
     A multi-line list of ``KEY=value`` settings which is used to set
     environment variables for the container. The variables are only available
     to the container, not to other containers or the test environment.
 
-``ports``
+``expose``
     A multi-line list of port mapping specifications, as
-    ``HOST_PORT:CONTAINER_PORT/PROTO``, which causes the container's
-    ``EXPOSE`` d port to be available on ``HOST_PORT``. See below for
-    more on port mapping.
-
-    If ``ports`` is not specified, all the container's ``EXPOSE`` d ports are
-    mapped (equivalent to ``docker run -P ...``)
-
-    For each mapped port, an environment variable of the form
-    ``<container-name>_<port-number>_<protocol>_PORT`` (eg
-    ``NGINX_80_TCP_PORT`` or ``TELEGRAF_8092_UDP_PORT``) is set for the test
-    run.
-
-    For each container, an environment variable of the form
-    ``<container_name>_HOST`` is set for the test run, indicating the host
-    name or IP address to use to communicate with the container.
-
-    If you set the ``HOST_PORT`` to zero, a random available port will be
-    assigned on the tox host. This is useful in case the container does not
-    ``EXPOSE`` the port you need, or if you want to map only some of the
-    ``EXPOSE``\d ports.
-
-    In both environment variables, the container name part is converted to
-    upper case, and all non-alphanumeric characters are replaced with an
+    ``ENV_VAR=CONTAINER_PORT/PROTO``. Within the testenv, the environment
+    variable ``ENV_VAR`` will contain the port number to connect to the
+    docker container's ``EXPOSE`` d port. If ``expose`` is specified, only
+    the listed ports will have environment variables created for them.
+
+    If ``expose`` is not specified, all the container's ``EXPOSE`` d ports
+    are made available (equivalent to ``docker run -P ...``) using default
+    environment variable names of the form
+    ``<container-name>_<port-number>_<protocol>_PORT`` (eg ``NGINX_80_TCP_PORT``
+    or ``TELEGRAF_8092_UDP_PORT``), with the container name and protocol
+    converted to upper case, and non-alphanumeric characters replaced with an
     underscore (``_``).
 
-    Tox-docker does not attempt to ensure that you have proper permission to
-    bind the ``HOST_PORT``, that it is not already bound and listening, etc;
-    if you explicitly list ports, it is your responsibility to ensure that
-    it can be successfully mapped.
+``host_var``
+    The name of an environment variable that will contain the hostname or IP
+    address to use to communicate with the container. Defaults to
+    ``<container_name>_HOST`` if not set, with the container name converted to
+    upper case, and non-alphanumeric characters replaced with an underscore
+    (``_``).
 
 ``links``
     A multi-line list of `container links
     <https://docs.docker.com/network/links/>`__, as ``other-container-name``
     or ``other-container-name:alias``. If no alias is given, the
     ``other-container-name`` is used. Within the container, the ``EXPOSE`` d
     ports of the other container will be available via the alias as hostname.
@@ -146,15 +136,15 @@
     and ``inside_path`` must be absolute paths.
 
 ``healthcheck_cmd``, ``healthcheck_interval``, ``healthcheck_retries``, ``healthcheck_start_period``, ``healthcheck_timeout``
     These set or customize parameters of the container `health check
     <https://docs.docker.com/engine/reference/builder/#healthcheck>`__. The
     ``healthcheck_interval``, ``healthcheck_start_period``, and
     ``healthcheck_timeout`` are specified as a number of seconds.
-    The ``healtcheck_cmd`` is an argv list which must name a command and
+    ``healthcheck_cmd`` is an argv list which must name a command and
     arguments that can be run within the container; if not specified, any
     health check built in to the container is used.
 
     If any healthcheck parameters are defined, tox-docker will delay the
     test run until the container reports healthy, and will fail the test
     run if it never does so (within the parameters specified).
 
@@ -222,40 +212,57 @@
 
     [docker:appserv]
     # You can use any value that `docker run` would accept as the image
     image = your-registry.example.org:1234/your-appserv
     # Within the appserv container, host "db" is linked to the postgres container
     links =
         db:db
-    # Use ports to expose specific ports; if you don't specify ports, then all
-    # the EXPOSEd ports defined by the image are mapped to an available
-    # ephemeral port.
-    ports =
-        8080:8080/tcp
+    # Expose ports to the testenv
+    expose =
+        APP_HTTP_PORT=8080/tcp
 
 
 Environment Variables
 ---------------------
 
 If you are running in a Docker-In-Docker environment, you can override the address
 used for port checking using the environment variable ``TOX_DOCKER_GATEWAY``. This
 variable should be the hostname or ip address used to connect to the container.
 
 Version Compatibility
 ---------------------
 
-Tox-docker requires tox to be run in Python 3.7 or newer, and requires tox
-version 3.0 or newer. Older versions of tox-docker may work with older
+Tox-docker requires tox to be run in Python 3.8 or newer, and requires tox
+version 4 or newer. Older versions of tox-docker may work with older
 versions of Python or tox, but these configurations are no longer supported.
 
+Upgrading
+---------
+
+Some configuration options were removed:
+
+New in 5.0:
+
+``ports``
+    This directive was removed in tox-docker version 5.0. Use ``expose``
+    instead. The ability to map a container port to a specific host port was
+    completely removed.
+
 
 ==========
 Change Log
 ==========
 
+* 5.0.0
+    * Remove support for tox 3
+    * Removed support for Python 3.7 and earlier
+    * Remove ``ports``; add ``expose`` and ``host_var``
+    * Support ``docker`` (the Python module) 7.x (thanks @jonathangreen)
+* 4.1.1
+    * Fix typo in README (thanks @akx)
 * 4.1.0
     * Drop test support for docker (Python library) 3.x; add test support
       for docker 6.x. Other versions may work, but we only support tested
       versions.
     * Add support for ``dockerfile`` and ``dockerfile_target`` directives
       to build local images
 * 4.0.0
@@ -282,17 +289,15 @@
 Development
 ===========
 
 Code Style
 ----------
 
 Tox-docker uses black and isort to enforce style standards on the codebase.
-The formatting is orindaily done for you via `pre-commit
+The formatting is ordinarily done for you via `pre-commit
 <https://pre-commit.com/>`_, and is enforced via the ``tox -e style`` build.
 To work on tox-docker locally with pre-commit, `pip install -r
 dev-requirements.txt`` and ``pre-commit install`` to set up the git hooks;
 subsequently, when you ``git commit``, the formatter will be run. If the
 changed files are not conformant, the hook will have reformatted them and
 you may need to run pre-commit again. You can run ``pre-commit run --files
 *.py`` to manually run the formatters.
-
-
```

### Comparing `tox-docker-4.1.0/tox_docker.egg-info/SOURCES.txt` & `tox_docker-5.0.0/tox_docker.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 version.txt
 tox_docker/__init__.py
 tox_docker/config.py
-tox_docker/log.py
 tox_docker/plugin.py
 tox_docker.egg-info/PKG-INFO
 tox_docker.egg-info/SOURCES.txt
 tox_docker.egg-info/dependency_links.txt
 tox_docker.egg-info/entry_points.txt
 tox_docker.egg-info/requires.txt
 tox_docker.egg-info/top_level.txt
@@ -20,16 +19,8 @@
 tox_docker/tests/test_env_vars.py
 tox_docker/tests/test_gateway.py
 tox_docker/tests/test_healthcheck.py
 tox_docker/tests/test_images.py
 tox_docker/tests/test_links.py
 tox_docker/tests/test_ports.py
 tox_docker/tests/test_volumes.py
-tox_docker/tests/util.py
-tox_docker/tox3/__init__.py
-tox_docker/tox3/config.py
-tox_docker/tox3/log.py
-tox_docker/tox3/plugin.py
-tox_docker/tox4/__init__.py
-tox_docker/tox4/config.py
-tox_docker/tox4/log.py
-tox_docker/tox4/plugin.py
+tox_docker/tests/util.py
```


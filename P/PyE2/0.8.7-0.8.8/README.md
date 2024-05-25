# Comparing `tmp/pye2-0.8.7.tar.gz` & `tmp/pye2-0.8.8.tar.gz`

## Comparing `pye2-0.8.7.tar` & `pye2-0.8.8.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pye2-0.8.7/.gitattributes
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pye2-0.8.7/TODOs.md
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pye2-0.8.7/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pye2-0.8.7/requirements.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.8.7/winrun.bat
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 pye2-0.8.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/__init__.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/_ver.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/base_decentra_object.py
--rw-r--r--   0        0        0     9060 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/plugins_manager_mixin.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/base/__init__.py
--rw-r--r--   0        0        0    51291 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/base/generic_session.py
--rw-r--r--   0        0        0    14080 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/base/instance.py
--rw-r--r--   0        0        0    49643 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/base/pipeline.py
--rw-r--r--   0        0        0   129442 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/base/plugin_template.py
--rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/base/responses.py
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/base/transaction.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/base/payload/__init__.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/base/payload/payload.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/bc/__init__.py
--rw-r--r--   0        0        0    27458 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/bc/base.py
--rw-r--r--   0        0        0     7579 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/bc/ec.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/code_cheker/__init__.py
--rw-r--r--   0        0        0    12913 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/code_cheker/base.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/comm/__init__.py
--rw-r--r--   0        0        0     8535 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/comm/amqp_wrapper.py
--rw-r--r--   0        0        0    13823 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/comm/mqtt_wrapper.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/const/README.md
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/const/__init__.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/const/base.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/const/comms.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/const/environment.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/const/formatter.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/const/heartbeat.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/const/misc.py
--rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/const/payload.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/default/__init__.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/default/mqtt_session.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/io_formatter/__init__.py
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/io_formatter/io_formatter_manager.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/io_formatter/base/__init__.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/io_formatter/base/base_formatter.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/io_formatter/default/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/io_formatter/default/a_dummy.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/io_formatter/default/aixp1.py
--rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/io_formatter/default/cavi2.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/io_formatter/default/default.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/__init__.py
--rw-r--r--   0        0        0    59434 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/base_logger.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/small_logger.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/logger_mixins/__init__.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/logger_mixins/class_instance_mixin.py
--rw-r--r--   0        0        0    13213 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/logger_mixins/computer_vision_mixin.py
--rw-r--r--   0        0        0    11258 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/logger_mixins/datetime_mixin.py
--rw-r--r--   0        0        0    13109 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/logger_mixins/download_mixin.py
--rw-r--r--   0        0        0     7420 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/logger_mixins/general_serialization_mixin.py
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/logger_mixins/json_serialization_mixin.py
--rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/logger_mixins/pickle_serialization_mixin.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/logger_mixins/process_mixin.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/logger_mixins/resource_size_mixin.py
--rw-r--r--   0        0        0    17133 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/logger_mixins/timers_mixin.py
--rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/logger_mixins/upload_mixin.py
--rw-r--r--   0        0        0    19342 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/logger_mixins/utils_mixin.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/tzlocal/__init__.py
--rw-r--r--   0        0        0     7268 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/tzlocal/unix.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/tzlocal/utils.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/tzlocal/win32.py
--rw-r--r--   0        0        0    34203 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/logging/tzlocal/windows_tz.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/tutorials/.example_env
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/tutorials/1. hello_world.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/tutorials/2. first_deploy.py
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/tutorials/3. simple_real_time_custom_code.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/tutorials/4. real_time_custom_code_2.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/tutorials/5. real_time_custom_code_multithreading.py
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/tutorials/6. real_time_custom_code_multithreading_extra.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/tutorials/7. real_time_custom_code_multithreading.py
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/tutorials/8. chatbot.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/utils/__init__.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/utils/code.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/utils/code_exec.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/utils/comm_utils.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 pye2-0.8.7/PyE2/utils/dotenv.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.8.7/xperimental/.example_env
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 pye2-0.8.7/xperimental/attach_example.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 pye2-0.8.7/xperimental/ex1.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pye2-0.8.7/xperimental/hello.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 pye2-0.8.7/xperimental/remote_exec.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pye2-0.8.7/xperimental/save_images.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.8.7/xperimental/_archive/test.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 pye2-0.8.7/xperimental/decentralized/chain_dist_example.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pye2-0.8.7/xperimental/decentralized/chain_dist_example_initiator.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.8.7/xperimental/decentralized/chain_dist_example_worker.py
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 pye2-0.8.7/xperimental/utils/get_documentation.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 pye2-0.8.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.8.7/LICENSE
--rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 pye2-0.8.7/README.md
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 pye2-0.8.7/pyproject.toml
--rw-r--r--   0        0        0    12845 2020-02-02 00:00:00.000000 pye2-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pye2-0.8.8/.gitattributes
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pye2-0.8.8/TODOs.md
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 pye2-0.8.8/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pye2-0.8.8/requirements.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pye2-0.8.8/winrun.bat
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 pye2-0.8.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/__init__.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/_ver.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/base_decentra_object.py
+-rw-r--r--   0        0        0     9060 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/plugins_manager_mixin.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/base/__init__.py
+-rw-r--r--   0        0        0    51291 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/base/generic_session.py
+-rw-r--r--   0        0        0    14048 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/base/instance.py
+-rw-r--r--   0        0        0    49748 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/base/pipeline.py
+-rw-r--r--   0        0        0   129442 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/base/plugin_template.py
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/base/responses.py
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/base/transaction.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/base/payload/__init__.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/base/payload/payload.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/bc/__init__.py
+-rw-r--r--   0        0        0    27458 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/bc/base.py
+-rw-r--r--   0        0        0     7579 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/bc/ec.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/code_cheker/__init__.py
+-rw-r--r--   0        0        0    12913 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/code_cheker/base.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/comm/__init__.py
+-rw-r--r--   0        0        0     8535 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/comm/amqp_wrapper.py
+-rw-r--r--   0        0        0    13823 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/comm/mqtt_wrapper.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/const/README.md
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/const/__init__.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/const/base.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/const/comms.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/const/environment.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/const/formatter.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/const/heartbeat.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/const/misc.py
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/const/payload.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/default/__init__.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/default/mqtt_session.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/io_formatter/__init__.py
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/io_formatter/io_formatter_manager.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/io_formatter/base/__init__.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/io_formatter/base/base_formatter.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/io_formatter/default/__init__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/io_formatter/default/a_dummy.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/io_formatter/default/aixp1.py
+-rw-r--r--   0        0        0    10492 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/io_formatter/default/cavi2.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/io_formatter/default/default.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/__init__.py
+-rw-r--r--   0        0        0    59434 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/base_logger.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/small_logger.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/logger_mixins/__init__.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/logger_mixins/class_instance_mixin.py
+-rw-r--r--   0        0        0    13213 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/logger_mixins/computer_vision_mixin.py
+-rw-r--r--   0        0        0    11258 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/logger_mixins/datetime_mixin.py
+-rw-r--r--   0        0        0    13109 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/logger_mixins/download_mixin.py
+-rw-r--r--   0        0        0     7420 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/logger_mixins/general_serialization_mixin.py
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/logger_mixins/json_serialization_mixin.py
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/logger_mixins/pickle_serialization_mixin.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/logger_mixins/process_mixin.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/logger_mixins/resource_size_mixin.py
+-rw-r--r--   0        0        0    17133 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/logger_mixins/timers_mixin.py
+-rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/logger_mixins/upload_mixin.py
+-rw-r--r--   0        0        0    19342 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/logger_mixins/utils_mixin.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/tzlocal/__init__.py
+-rw-r--r--   0        0        0     7268 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/tzlocal/unix.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/tzlocal/utils.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/tzlocal/win32.py
+-rw-r--r--   0        0        0    34203 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/logging/tzlocal/windows_tz.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/tutorials/.example_env
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/tutorials/1. hello_world.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/tutorials/2. first_deploy.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/tutorials/3. simple_real_time_custom_code.py
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/tutorials/4. real_time_custom_code_2.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/tutorials/5. real_time_custom_code_multithreading.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/tutorials/6. real_time_custom_code_multithreading_extra.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/tutorials/7. real_time_custom_code_multithreading.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/tutorials/8. chatbot.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/utils/__init__.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/utils/code.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/utils/code_exec.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/utils/comm_utils.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 pye2-0.8.8/PyE2/utils/dotenv.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pye2-0.8.8/xperimental/.example_env
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 pye2-0.8.8/xperimental/attach_example.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 pye2-0.8.8/xperimental/ex1.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pye2-0.8.8/xperimental/hello.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 pye2-0.8.8/xperimental/remote_exec.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pye2-0.8.8/xperimental/save_images.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pye2-0.8.8/xperimental/_archive/test.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 pye2-0.8.8/xperimental/decentralized/chain_dist_example.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 pye2-0.8.8/xperimental/decentralized/chain_dist_example_initiator.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pye2-0.8.8/xperimental/decentralized/chain_dist_example_worker.py
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 pye2-0.8.8/xperimental/utils/get_documentation.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 pye2-0.8.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pye2-0.8.8/LICENSE
+-rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 pye2-0.8.8/README.md
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 pye2-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0    12845 2020-02-02 00:00:00.000000 pye2-0.8.8/PKG-INFO
```

### Comparing `pye2-0.8.7/.github/workflows/python-publish.yml` & `pye2-0.8.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/base_decentra_object.py` & `pye2-0.8.8/PyE2/base_decentra_object.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/plugins_manager_mixin.py` & `pye2-0.8.8/PyE2/plugins_manager_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/base/generic_session.py` & `pye2-0.8.8/PyE2/base/generic_session.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/base/instance.py` & `pye2-0.8.8/PyE2/base/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
     def was_last_operation_successful(self) -> bool:
       """
       Get the status of the last operation.
 
       Example:
       --------
       ```python
-      instance.send_instance_command("RESTART", wait_for_confirmation=False)
+      instance.send_instance_command("RESTART", wait_confirmation=False)
 
       if instance.was_last_operation_successful is not None:
         if instance.was_last_operation_successful:
           print("Last operation was successful")
         else:
           print("Last operation failed")
       else:
@@ -365,46 +365,46 @@
             del self.proposed_config[k]
 
       if len(self.proposed_config) == 0:
         self.proposed_config = None
 
       return
 
-    def send_instance_command(self, command, payload={}, command_params={}, wait_for_confirmation=True, timeout=10):
+    def send_instance_command(self, command, payload={}, command_params={}, wait_confirmation=True, timeout=10):
       """
       Send a command to the instance.
       This command can block until the command is confirmed by the DecentrAI node.
 
       Example:
       --------
       ```python
-      instance.send_instance_command('START', wait_for_confirmation=True)
+      instance.send_instance_command('START', wait_confirmation=True)
 
-      transactions_p1 = instance1.send_instance_command('START', wait_for_confirmation=False)
-      transactions_p2 = instance2.send_instance_command('START', wait_for_confirmation=False)
+      transactions_p1 = instance1.send_instance_command('START', wait_confirmation=False)
+      transactions_p2 = instance2.send_instance_command('START', wait_confirmation=False)
       # wait for both commands to be confirmed, but after both commands are sent
       session.wait_for_transactions(transactions_p1 + transactions_p2)
       ```
       Parameters
       ----------
       command : str
           The command to send
       payload : dict, optional
           The payload of the command, by default {}
       command_params : dict, optional
           The parameters of the command, by default {}
-      wait_for_confirmation : bool, optional
+      wait_confirmation : bool, optional
           Whether to wait for the confirmation of the command, by default False
       timeout : int, optional
           The timeout for the transaction, by default 10    
 
       Returns
       -------
       list[Transaction] | None
-          The list of transactions generated, or None if `wait_for_confirmation` is False.
+          The list of transactions generated, or None if `wait_confirmation` is False.
 
       """
       self.P(f'Sending command <{command}> to instance <{self.__repr__()}>', color="b")
 
       self.__was_last_operation_successful = None
 
       transactions = self.__register_transaction_for_instance_command(timeout=timeout)
@@ -415,15 +415,15 @@
         signature=self.signature,
         instance_id=self.instance_id,
         command=command,
         payload=payload,
         command_params=command_params,
       )
 
-      if wait_for_confirmation:
+      if wait_confirmation:
         self.pipeline.session.wait_for_transactions(transactions)
       else:
         return transactions
       return
 
     def close(self):
       """
```

### Comparing `pye2-0.8.7/PyE2/base/pipeline.py` & `pye2-0.8.8/PyE2/base/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,15 @@
       for instance in self.lst_plugin_instances:
         if instance._is_tainted():
           transactions.append(self.session._register_transaction(
             session_id=session_id,
             lst_required_responses=instance._get_instance_update_required_responses(),
             timeout=timeout,
             on_success_callback=instance._apply_staged_config,
+            # TODO: if the instance was newly added, remove it from the tracked list
             on_failure_callback=instance._discard_staged_config,
           ))
       # end for register to update instances
 
       for instance in self.proposed_remove_instances:
         transactions.append(self.session._register_transaction(
           session_id=session_id,
@@ -552,24 +553,24 @@
       for instance in self.lst_plugin_instances:
         if instance._is_tainted():
           self.P("  - Plugin <{}:{}>:".format(instance.signature, instance.instance_id), verbosity=1)
           self.P("    - Current config: {}".format(instance.config), verbosity=1)
           self.P("    - Proposed config: {}".format(instance.proposed_config), verbosity=1)
       return
 
-    def _close(self):
+    def _close(self, timeout=10):
       """
       Close the pipeline.
 
       Returns
       -------
       list[Transaction]
           The list of transactions generated.
       """
-      transactions = self.__register_transactions_for_delete(timeout=10)
+      transactions = self.__register_transactions_for_delete(timeout=timeout)
 
       self.session._send_command_archive_pipeline(
         worker=self.node_id,
         pipeline_name=self.name,
       )
 
       return transactions
@@ -955,22 +956,23 @@
         pass
 
       # stop the stream
       instance.close()
 
       return result, error
 
-    def close(self):
+    def close(self, wait_confirmation=True, timeout=10):
       """
       Close the pipeline, stopping all the instances associated with it.
       """
 
-      transactions = self._close()
+      transactions = self._close(timeout=timeout)
 
-      self.session.wait_for_transactions(transactions)
+      if wait_confirmation:
+        self.session.wait_for_transactions(transactions)
       return
 
     def P(self, *args, **kwargs):
       """
       Print info to stdout.
       """
       return self.log.P(*args, **kwargs)
@@ -1103,60 +1105,59 @@
             del self.proposed_config[k]
 
       if len(self.proposed_config) == 0:
         self.proposed_config = None
 
       return
 
-    def send_pipeline_command(self, command, payload={}, command_params={}, wait_for_confirmation=True, timeout=10) -> list[Transaction]:
-      # TODO: test if pipeline command works okay
+    def send_pipeline_command(self, command, payload={}, command_params={}, wait_confirmation=True, timeout=10) -> list[Transaction]:
       """
       Send a pipeline command to the DecentrAI node.
       This command can block until the command is confirmed by the DecentrAI node.
 
       Example:
       --------
       ```python
-      pipeline.send_pipeline_command('START', wait_for_confirmation=True)
+      pipeline.send_pipeline_command('START', wait_confirmation=True)
 
-      transactions_p1 = pipeline1.send_pipeline_command('START', wait_for_confirmation=False)
-      transactions_p2 = pipeline2.send_pipeline_command('START', wait_for_confirmation=False)
+      transactions_p1 = pipeline1.send_pipeline_command('START', wait_confirmation=False)
+      transactions_p2 = pipeline2.send_pipeline_command('START', wait_confirmation=False)
       # wait for both commands to be confirmed, but after both commands are sent
       session.wait_for_transactions(transactions_p1 + transactions_p2)
       ```
 
       Parameters
       ----------
       command : str
           The name of the command.
       payload : dict, optional
           The payload of the command, by default {}
       command_params : dict, optional
           The parameters of the command, by default {}
-      wait_for_confirmation : bool, optional
+      wait_confirmation : bool, optional
           Whether to wait for the confirmation of the command, by default False
       timeout : int, optional
           The timeout for the transaction, by default 10    
 
       Returns
       -------
       list[Transaction] | None
-          The list of transactions generated, or None if `wait_for_confirmation` is False.
+          The list of transactions generated, or None if `wait_confirmation` is False.
       """
       transactions = self.__register_transaction_for_pipeline_command(timeout=timeout)
 
       self.session._send_command_pipeline_command(
         worker=self.node_id,
         pipeline_name=self.name,
         command=command,
         payload=payload,
         command_params=command_params,
       )
 
-      if wait_for_confirmation:
+      if wait_confirmation:
         self.session.wait_for_transactions(transactions)
       else:
         return transactions
       return
 
     def create_or_attach_to_plugin_instance(self, *, signature, instance_id, config={}, on_data=None, on_notification=None, **kwargs) -> Instance:
       """
```

### Comparing `pye2-0.8.7/PyE2/base/plugin_template.py` & `pye2-0.8.8/PyE2/base/plugin_template.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/base/responses.py` & `pye2-0.8.8/PyE2/base/responses.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/base/transaction.py` & `pye2-0.8.8/PyE2/base/transaction.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/base/payload/payload.py` & `pye2-0.8.8/PyE2/base/payload/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/bc/base.py` & `pye2-0.8.8/PyE2/bc/base.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/bc/ec.py` & `pye2-0.8.8/PyE2/bc/ec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/code_cheker/base.py` & `pye2-0.8.8/PyE2/code_cheker/base.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/comm/amqp_wrapper.py` & `pye2-0.8.8/PyE2/comm/amqp_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/comm/mqtt_wrapper.py` & `pye2-0.8.8/PyE2/comm/mqtt_wrapper.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/const/base.py` & `pye2-0.8.8/PyE2/const/base.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/const/comms.py` & `pye2-0.8.8/PyE2/const/comms.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/const/heartbeat.py` & `pye2-0.8.8/PyE2/const/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/const/payload.py` & `pye2-0.8.8/PyE2/const/payload.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/default/mqtt_session.py` & `pye2-0.8.8/PyE2/default/mqtt_session.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/io_formatter/io_formatter_manager.py` & `pye2-0.8.8/PyE2/io_formatter/io_formatter_manager.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/io_formatter/base/base_formatter.py` & `pye2-0.8.8/PyE2/io_formatter/base/base_formatter.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/io_formatter/default/a_dummy.py` & `pye2-0.8.8/PyE2/io_formatter/default/a_dummy.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/io_formatter/default/aixp1.py` & `pye2-0.8.8/PyE2/io_formatter/default/aixp1.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/io_formatter/default/cavi2.py` & `pye2-0.8.8/PyE2/io_formatter/default/cavi2.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/base_logger.py` & `pye2-0.8.8/PyE2/logging/base_logger.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/small_logger.py` & `pye2-0.8.8/PyE2/logging/small_logger.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/logger_mixins/__init__.py` & `pye2-0.8.8/PyE2/logging/logger_mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/logger_mixins/class_instance_mixin.py` & `pye2-0.8.8/PyE2/logging/logger_mixins/class_instance_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/logger_mixins/computer_vision_mixin.py` & `pye2-0.8.8/PyE2/logging/logger_mixins/computer_vision_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/logger_mixins/datetime_mixin.py` & `pye2-0.8.8/PyE2/logging/logger_mixins/datetime_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/logger_mixins/download_mixin.py` & `pye2-0.8.8/PyE2/logging/logger_mixins/download_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/logger_mixins/general_serialization_mixin.py` & `pye2-0.8.8/PyE2/logging/logger_mixins/general_serialization_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/logger_mixins/json_serialization_mixin.py` & `pye2-0.8.8/PyE2/logging/logger_mixins/json_serialization_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/logger_mixins/pickle_serialization_mixin.py` & `pye2-0.8.8/PyE2/logging/logger_mixins/pickle_serialization_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/logger_mixins/process_mixin.py` & `pye2-0.8.8/PyE2/logging/logger_mixins/process_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/logger_mixins/resource_size_mixin.py` & `pye2-0.8.8/PyE2/logging/logger_mixins/resource_size_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/logger_mixins/timers_mixin.py` & `pye2-0.8.8/PyE2/logging/logger_mixins/timers_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/logger_mixins/upload_mixin.py` & `pye2-0.8.8/PyE2/logging/logger_mixins/upload_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/logger_mixins/utils_mixin.py` & `pye2-0.8.8/PyE2/logging/logger_mixins/utils_mixin.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/tzlocal/unix.py` & `pye2-0.8.8/PyE2/logging/tzlocal/unix.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/tzlocal/utils.py` & `pye2-0.8.8/PyE2/logging/tzlocal/utils.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/tzlocal/win32.py` & `pye2-0.8.8/PyE2/logging/tzlocal/win32.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/logging/tzlocal/windows_tz.py` & `pye2-0.8.8/PyE2/logging/tzlocal/windows_tz.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/tutorials/1. hello_world.py` & `pye2-0.8.8/PyE2/tutorials/1. hello_world.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/tutorials/2. first_deploy.py` & `pye2-0.8.8/PyE2/tutorials/2. first_deploy.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/tutorials/3. simple_real_time_custom_code.py` & `pye2-0.8.8/PyE2/tutorials/3. simple_real_time_custom_code.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/tutorials/4. real_time_custom_code_2.py` & `pye2-0.8.8/PyE2/tutorials/4. real_time_custom_code_2.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/tutorials/5. real_time_custom_code_multithreading.py` & `pye2-0.8.8/PyE2/tutorials/5. real_time_custom_code_multithreading.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/tutorials/6. real_time_custom_code_multithreading_extra.py` & `pye2-0.8.8/PyE2/tutorials/6. real_time_custom_code_multithreading_extra.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/tutorials/7. real_time_custom_code_multithreading.py` & `pye2-0.8.8/PyE2/tutorials/7. real_time_custom_code_multithreading.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/tutorials/8. chatbot.py` & `pye2-0.8.8/PyE2/tutorials/8. chatbot.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/utils/code.py` & `pye2-0.8.8/PyE2/utils/code.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/utils/code_exec.py` & `pye2-0.8.8/PyE2/utils/code_exec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/utils/comm_utils.py` & `pye2-0.8.8/PyE2/utils/comm_utils.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/PyE2/utils/dotenv.py` & `pye2-0.8.8/PyE2/utils/dotenv.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/xperimental/attach_example.py` & `pye2-0.8.8/xperimental/attach_example.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/xperimental/ex1.py` & `pye2-0.8.8/xperimental/ex1.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/xperimental/remote_exec.py` & `pye2-0.8.8/xperimental/remote_exec.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/xperimental/save_images.py` & `pye2-0.8.8/xperimental/save_images.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/xperimental/decentralized/chain_dist_example.py` & `pye2-0.8.8/xperimental/decentralized/chain_dist_example.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/xperimental/decentralized/chain_dist_example_initiator.py` & `pye2-0.8.8/xperimental/decentralized/chain_dist_example_initiator.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/xperimental/utils/get_documentation.py` & `pye2-0.8.8/xperimental/utils/get_documentation.py`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/.gitignore` & `pye2-0.8.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/LICENSE` & `pye2-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/README.md` & `pye2-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `pye2-0.8.7/pyproject.toml` & `pye2-0.8.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyE2"
-version = "0.8.7"
+version = "0.8.8"
 authors = [
   { name="Stefan Saraev", email="saraevstefan@gmail.com" },
   { name="Andrei Ionut Damian", email="andrei.damian@me.com" },
   { name="Cristan Bleotiu", email="cristibleotiu@gmail.com" },
 ]
 description = "PyE2 is the Python SDK required for client app development in the DecentrAI network"
 readme = "README.md"
```

### Comparing `pye2-0.8.7/PKG-INFO` & `pye2-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: PyE2
-Version: 0.8.7
+Version: 0.8.8
 Summary: PyE2 is the Python SDK required for client app development in the DecentrAI network
 Project-URL: Homepage, https://github.com/DecentrAI/PyE2
 Project-URL: Bug Tracker, https://github.com/DecentrAI/PyE2/issues
 Author-email: Stefan Saraev <saraevstefan@gmail.com>, Andrei Ionut Damian <andrei.damian@me.com>, Cristan Bleotiu <cristibleotiu@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


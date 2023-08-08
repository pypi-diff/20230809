# Comparing `tmp/zaber_motion-4.2.4.tar.gz` & `tmp/zaber_motion-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaber_motion-4.2.4.tar", last modified: Tue Jul 25 16:25:56 2023, max compression
+gzip compressed data, was "zaber_motion-4.2.5.tar", last modified: Tue Aug  8 20:12:50 2023, max compression
```

## Comparing `zaber_motion-4.2.4.tar` & `zaber_motion-4.2.5.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.625079 zaber_motion-4.2.4/
--rw-r--r--   0 zaber      (501) staff       (20)      218 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/DESCRIPTION.md
--rw-r--r--   0 zaber      (501) staff       (20)   109244 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/LICENSE.txt
--rw-r--r--   0 zaber      (501) staff       (20)       13 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/MANIFEST.in
--rw-r--r--   0 zaber      (501) staff       (20)      808 2023-07-25 16:25:56.625141 zaber_motion-4.2.4/PKG-INFO
--rw-r--r--   0 zaber      (501) staff       (20)      218 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/README.md
--rw-r--r--   0 zaber      (501) staff       (20)      134 2023-07-25 16:25:56.625362 zaber_motion-4.2.4/setup.cfg
--rw-r--r--   0 zaber      (501) staff       (20)     1371 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/setup.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.604339 zaber_motion-4.2.4/test/
--rw-r--r--   0 zaber      (501) staff       (20)     3544 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/test/test_integration.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.606130 zaber_motion-4.2.4/zaber_motion/
--rw-r--r--   0 zaber      (501) staff       (20)     6583 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/__init__.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.613234 zaber_motion-4.2.4/zaber_motion/ascii/
--rw-r--r--   0 zaber      (501) staff       (20)     3136 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     2185 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/alert_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     8708 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/all_axes.py
--rw-r--r--   0 zaber      (501) staff       (20)    41649 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/axis.py
--rw-r--r--   0 zaber      (501) staff       (20)     2259 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/axis_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)    12952 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/axis_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      272 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     1265 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/can_set_state_axis_response.py
--rw-r--r--   0 zaber      (501) staff       (20)     1530 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/can_set_state_device_response.py
--rw-r--r--   0 zaber      (501) staff       (20)    34796 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/connection.py
--rw-r--r--   0 zaber      (501) staff       (20)     1959 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/conversion_factor.py
--rw-r--r--   0 zaber      (501) staff       (20)    24816 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/device.py
--rw-r--r--   0 zaber      (501) staff       (20)     2801 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/device_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)    17751 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/device_io.py
--rw-r--r--   0 zaber      (501) staff       (20)     2077 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/device_io_info.py
--rw-r--r--   0 zaber      (501) staff       (20)    12120 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/device_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/io_port_type.py
--rw-r--r--   0 zaber      (501) staff       (20)    37243 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/lockstep.py
--rw-r--r--   0 zaber      (501) staff       (20)     1671 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/lockstep_axes.py
--rw-r--r--   0 zaber      (501) staff       (20)      386 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/message_type.py
--rw-r--r--   0 zaber      (501) staff       (20)    17493 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/oscilloscope.py
--rw-r--r--   0 zaber      (501) staff       (20)     2423 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/oscilloscope_capture_properties.py
--rw-r--r--   0 zaber      (501) staff       (20)     5695 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/oscilloscope_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      268 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/oscilloscope_data_source.py
--rw-r--r--   0 zaber      (501) staff       (20)     1601 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/paramset_info.py
--rw-r--r--   0 zaber      (501) staff       (20)     2078 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/pid_tuning.py
--rw-r--r--   0 zaber      (501) staff       (20)    26067 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/process.py
--rw-r--r--   0 zaber      (501) staff       (20)     3830 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/process_controller.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/process_controller_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     2074 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/process_controller_source.py
--rw-r--r--   0 zaber      (501) staff       (20)      281 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/process_controller_source_sensor.py
--rw-r--r--   0 zaber      (501) staff       (20)     2071 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/pvt_axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)      256 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/pvt_axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3190 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/pvt_buffer.py
--rw-r--r--   0 zaber      (501) staff       (20)      247 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/pvt_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)    33707 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/pvt_sequence.py
--rw-r--r--   0 zaber      (501) staff       (20)     2896 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/response.py
--rw-r--r--   0 zaber      (501) staff       (20)    19220 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/servo_tuner.py
--rw-r--r--   0 zaber      (501) staff       (20)     1782 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/servo_tuning_param.py
--rw-r--r--   0 zaber      (501) staff       (20)      384 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/servo_tuning_paramset.py
--rw-r--r--   0 zaber      (501) staff       (20)    23693 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/setting_constants.py
--rw-r--r--   0 zaber      (501) staff       (20)     1893 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/simple_tuning_param_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)    26082 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/storage.py
--rw-r--r--   0 zaber      (501) staff       (20)    85042 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/stream.py
--rw-r--r--   0 zaber      (501) staff       (20)     2110 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/stream_axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)      253 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/stream_axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3084 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/stream_buffer.py
--rw-r--r--   0 zaber      (501) staff       (20)      273 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/stream_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     5345 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/transport.py
--rw-r--r--   0 zaber      (501) staff       (20)     2966 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/unknown_response_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     2855 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/warning_flags.py
--rw-r--r--   0 zaber      (501) staff       (20)     5066 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/ascii/warnings.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.614672 zaber_motion-4.2.4/zaber_motion/binary/
--rw-r--r--   0 zaber      (501) staff       (20)      653 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     1940 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/binary_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)     3132 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/command_code.py
--rw-r--r--   0 zaber      (501) staff       (20)    19670 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/connection.py
--rw-r--r--   0 zaber      (501) staff       (20)    29083 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/device.py
--rw-r--r--   0 zaber      (501) staff       (20)     3361 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/device_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)     3513 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/device_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      276 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/device_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3116 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/error_code.py
--rw-r--r--   0 zaber      (501) staff       (20)     1498 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/message.py
--rw-r--r--   0 zaber      (501) staff       (20)      415 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/reply_code.py
--rw-r--r--   0 zaber      (501) staff       (20)     1552 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/reply_only_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     1588 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/binary/unknown_response_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     1515 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/bindings.py
--rw-r--r--   0 zaber      (501) staff       (20)     4187 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/call.py
--rw-r--r--   0 zaber      (501) staff       (20)     7349 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/convert_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      257 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/device_db_source_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     2190 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/events.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.623111 zaber_motion-4.2.4/zaber_motion/exceptions/
--rw-r--r--   0 zaber      (501) staff       (20)     7384 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     1121 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/binary_command_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      991 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/binary_command_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1045 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/command_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     3097 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/command_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/command_preempted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1129 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/command_too_long_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1971 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/command_too_long_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      304 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/connection_closed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/connection_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/conversion_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1158 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/device_address_conflict_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1126 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/device_address_conflict_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      314 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/device_busy_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1092 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/device_db_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      911 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/device_db_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      283 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/device_detection_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      335 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/device_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      317 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/device_not_identified_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1065 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/g_code_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1321 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/g_code_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1036 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/g_code_syntax_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1300 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/g_code_syntax_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      309 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/internal_error_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      295 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_argument_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      300 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_data_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      310 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_operation_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1058 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_packet_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1198 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_packet_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      282 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_park_state_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1140 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_pvt_point.py
--rw-r--r--   0 zaber      (501) staff       (20)     1091 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_response_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      928 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/invalid_response_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      342 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/io_channel_out_of_range_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      297 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/io_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      322 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/lockstep_enabled_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      329 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/lockstep_not_enabled_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      386 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/motion_lib_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1070 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1852 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1137 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1875 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/no_device_found_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      297 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/no_value_for_key_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/not_supported_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/os_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      317 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/out_of_request_ids_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      323 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_discontinuity_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1037 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1749 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      326 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_mode_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1102 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1292 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1169 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1327 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      285 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/pvt_setup_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      300 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/request_timeout_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      349 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/serial_port_busy_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     3563 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/set_device_state_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1085 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/set_device_state_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     2372 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/set_peripheral_state_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1120 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/setting_not_found_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      320 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_discontinuity_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1060 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1232 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      323 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_mode_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1134 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1313 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1199 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1348 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      282 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/stream_setup_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      341 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/timeout_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      320 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/transport_already_used_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      335 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/exceptions/unknown_request_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     2088 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/firmware_version.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.624249 zaber_motion-4.2.4/zaber_motion/gcode/
--rw-r--r--   0 zaber      (501) staff       (20)      578 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     2242 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)     1547 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/axis_mapping.py
--rw-r--r--   0 zaber      (501) staff       (20)     2139 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/axis_transformation.py
--rw-r--r--   0 zaber      (501) staff       (20)     2290 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/device_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)    12481 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/offline_translator.py
--rw-r--r--   0 zaber      (501) staff       (20)     1555 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/translate_message.py
--rw-r--r--   0 zaber      (501) staff       (20)     1401 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/translate_result.py
--rw-r--r--   0 zaber      (501) staff       (20)    13105 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/translator.py
--rw-r--r--   0 zaber      (501) staff       (20)     2206 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/gcode/translator_config.py
--rw-r--r--   0 zaber      (501) staff       (20)     2838 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/library.py
--rw-r--r--   0 zaber      (501) staff       (20)      279 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/log_output_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     1937 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/measurement.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.624473 zaber_motion-4.2.4/zaber_motion/microscopy/
--rw-r--r--   0 zaber      (501) staff       (20)       68 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/microscopy/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     7651 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/microscopy/objective_changer.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.624843 zaber_motion-4.2.4/zaber_motion/protobufs/
--rw-r--r--   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/protobufs/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)    67796 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/protobufs/main_pb2.py
--rw-r--r--   0 zaber      (501) staff       (20)   206754 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/protobufs/main_pb2.pyi
--rw-r--r--   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/py.typed
--rw-r--r--   0 zaber      (501) staff       (20)      278 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/rotation_direction.py
--rw-r--r--   0 zaber      (501) staff       (20)      987 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/serialization.py
--rw-r--r--   0 zaber      (501) staff       (20)     2108 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/tools.py
--rw-r--r--   0 zaber      (501) staff       (20)     9340 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/units.py
--rw-r--r--   0 zaber      (501) staff       (20)       22 2023-07-25 16:25:14.000000 zaber_motion-4.2.4/zaber_motion/version.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-07-25 16:25:56.606701 zaber_motion-4.2.4/zaber_motion.egg-info/
--rw-r--r--   0 zaber      (501) staff       (20)      808 2023-07-25 16:25:56.000000 zaber_motion-4.2.4/zaber_motion.egg-info/PKG-INFO
--rw-r--r--   0 zaber      (501) staff       (20)     7890 2023-07-25 16:25:56.000000 zaber_motion-4.2.4/zaber_motion.egg-info/SOURCES.txt
--rw-r--r--   0 zaber      (501) staff       (20)        1 2023-07-25 16:25:56.000000 zaber_motion-4.2.4/zaber_motion.egg-info/dependency_links.txt
--rw-r--r--   0 zaber      (501) staff       (20)      239 2023-07-25 16:25:56.000000 zaber_motion-4.2.4/zaber_motion.egg-info/requires.txt
--rw-r--r--   0 zaber      (501) staff       (20)       13 2023-07-25 16:25:56.000000 zaber_motion-4.2.4/zaber_motion.egg-info/top_level.txt
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-08-08 20:12:50.036941 zaber_motion-4.2.5/
+-rw-r--r--   0 zaber      (501) staff       (20)      218 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/DESCRIPTION.md
+-rw-r--r--   0 zaber      (501) staff       (20)   109244 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/LICENSE.txt
+-rw-r--r--   0 zaber      (501) staff       (20)       13 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/MANIFEST.in
+-rw-r--r--   0 zaber      (501) staff       (20)      808 2023-08-08 20:12:50.037013 zaber_motion-4.2.5/PKG-INFO
+-rw-r--r--   0 zaber      (501) staff       (20)      218 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/README.md
+-rw-r--r--   0 zaber      (501) staff       (20)      134 2023-08-08 20:12:50.037242 zaber_motion-4.2.5/setup.cfg
+-rw-r--r--   0 zaber      (501) staff       (20)     1371 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/setup.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-08-08 20:12:50.016676 zaber_motion-4.2.5/test/
+-rw-r--r--   0 zaber      (501) staff       (20)     3544 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/test/test_integration.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-08-08 20:12:50.018393 zaber_motion-4.2.5/zaber_motion/
+-rw-r--r--   0 zaber      (501) staff       (20)     6583 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/__init__.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-08-08 20:12:50.025230 zaber_motion-4.2.5/zaber_motion/ascii/
+-rw-r--r--   0 zaber      (501) staff       (20)     3136 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2185 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/alert_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     8708 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/all_axes.py
+-rw-r--r--   0 zaber      (501) staff       (20)    41649 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/axis.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2259 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/axis_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12952 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/axis_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      272 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1265 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/can_set_state_axis_response.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1530 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/can_set_state_device_response.py
+-rw-r--r--   0 zaber      (501) staff       (20)    34796 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/connection.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1959 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/conversion_factor.py
+-rw-r--r--   0 zaber      (501) staff       (20)    24816 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/device.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2801 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/device_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)    17751 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/device_io.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2077 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/device_io_info.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12120 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/device_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/io_port_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)    37243 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/lockstep.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1671 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/lockstep_axes.py
+-rw-r--r--   0 zaber      (501) staff       (20)      386 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/message_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)    17493 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/oscilloscope.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2423 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/oscilloscope_capture_properties.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5695 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/oscilloscope_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      268 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/oscilloscope_data_source.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1601 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/paramset_info.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2078 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/pid_tuning.py
+-rw-r--r--   0 zaber      (501) staff       (20)    26067 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/process.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3830 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/process_controller.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/process_controller_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2074 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/process_controller_source.py
+-rw-r--r--   0 zaber      (501) staff       (20)      281 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/process_controller_source_sensor.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2071 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/pvt_axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)      256 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/pvt_axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3190 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/pvt_buffer.py
+-rw-r--r--   0 zaber      (501) staff       (20)      247 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/pvt_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)    33707 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/pvt_sequence.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2896 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/response.py
+-rw-r--r--   0 zaber      (501) staff       (20)    19220 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/servo_tuner.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1782 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/servo_tuning_param.py
+-rw-r--r--   0 zaber      (501) staff       (20)      384 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/servo_tuning_paramset.py
+-rw-r--r--   0 zaber      (501) staff       (20)    23693 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/setting_constants.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1893 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/simple_tuning_param_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)    26082 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/storage.py
+-rw-r--r--   0 zaber      (501) staff       (20)    85042 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/stream.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2110 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/stream_axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)      253 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/stream_axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3084 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/stream_buffer.py
+-rw-r--r--   0 zaber      (501) staff       (20)      273 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/stream_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5345 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/transport.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2966 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/unknown_response_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2855 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/warning_flags.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5066 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/ascii/warnings.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-08-08 20:12:50.026672 zaber_motion-4.2.5/zaber_motion/binary/
+-rw-r--r--   0 zaber      (501) staff       (20)      653 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/binary/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1940 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/binary/binary_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3132 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/binary/command_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)    19670 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/binary/connection.py
+-rw-r--r--   0 zaber      (501) staff       (20)    29083 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/binary/device.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3361 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/binary/device_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3513 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/binary/device_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      276 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/binary/device_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3116 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/binary/error_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1498 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/binary/message.py
+-rw-r--r--   0 zaber      (501) staff       (20)      415 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/binary/reply_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1552 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/binary/reply_only_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1588 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/binary/unknown_response_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1515 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/bindings.py
+-rw-r--r--   0 zaber      (501) staff       (20)     4187 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/call.py
+-rw-r--r--   0 zaber      (501) staff       (20)     7349 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/convert_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      257 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/device_db_source_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2190 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/events.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-08-08 20:12:50.034959 zaber_motion-4.2.5/zaber_motion/exceptions/
+-rw-r--r--   0 zaber      (501) staff       (20)     7384 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1121 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/binary_command_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      991 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/binary_command_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1045 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/command_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3097 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/command_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/command_preempted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1129 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/command_too_long_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1971 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/command_too_long_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      304 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/connection_closed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/connection_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/conversion_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1158 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/device_address_conflict_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1126 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/device_address_conflict_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      314 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/device_busy_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1092 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/device_db_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      911 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/device_db_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      283 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/device_detection_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      335 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/device_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      317 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/device_not_identified_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1065 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/g_code_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1321 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/g_code_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1036 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/g_code_syntax_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1300 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/g_code_syntax_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      309 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/internal_error_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      295 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/invalid_argument_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      300 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/invalid_data_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      310 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/invalid_operation_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1058 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/invalid_packet_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1198 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/invalid_packet_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      282 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/invalid_park_state_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1140 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/invalid_pvt_point.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1091 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/invalid_response_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      928 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/invalid_response_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      342 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/io_channel_out_of_range_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      297 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/io_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      322 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/lockstep_enabled_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      329 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/lockstep_not_enabled_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      386 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/motion_lib_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1070 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1852 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1137 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1875 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/no_device_found_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      297 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/no_value_for_key_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/not_supported_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/os_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      317 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/out_of_request_ids_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      323 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/pvt_discontinuity_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1037 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/pvt_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1749 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/pvt_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      326 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/pvt_mode_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1102 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/pvt_movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1292 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/pvt_movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1169 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1327 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      285 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/pvt_setup_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      300 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/request_timeout_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      349 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/serial_port_busy_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3563 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/set_device_state_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1085 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/set_device_state_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2372 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/set_peripheral_state_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1120 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/setting_not_found_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      320 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/stream_discontinuity_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1060 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/stream_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1232 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/stream_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      323 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/stream_mode_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1134 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/stream_movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1313 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/stream_movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1199 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/stream_movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1348 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      282 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/stream_setup_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      341 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/timeout_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      320 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/transport_already_used_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      335 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/exceptions/unknown_request_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2088 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/firmware_version.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-08-08 20:12:50.036078 zaber_motion-4.2.5/zaber_motion/gcode/
+-rw-r--r--   0 zaber      (501) staff       (20)      578 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/gcode/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2242 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/gcode/axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1547 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/gcode/axis_mapping.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2139 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/gcode/axis_transformation.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2290 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/gcode/device_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12481 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/gcode/offline_translator.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1555 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/gcode/translate_message.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1401 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/gcode/translate_result.py
+-rw-r--r--   0 zaber      (501) staff       (20)    13105 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/gcode/translator.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2206 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/gcode/translator_config.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3346 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/library.py
+-rw-r--r--   0 zaber      (501) staff       (20)      279 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/log_output_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1937 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/measurement.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-08-08 20:12:50.036296 zaber_motion-4.2.5/zaber_motion/microscopy/
+-rw-r--r--   0 zaber      (501) staff       (20)       68 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/microscopy/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     7651 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/microscopy/objective_changer.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-08-08 20:12:50.036643 zaber_motion-4.2.5/zaber_motion/protobufs/
+-rw-r--r--   0 zaber      (501) staff       (20)        0 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/protobufs/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)    67921 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/protobufs/main_pb2.py
+-rw-r--r--   0 zaber      (501) staff       (20)   207174 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/protobufs/main_pb2.pyi
+-rw-r--r--   0 zaber      (501) staff       (20)        0 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/py.typed
+-rw-r--r--   0 zaber      (501) staff       (20)      278 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/rotation_direction.py
+-rw-r--r--   0 zaber      (501) staff       (20)      987 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/serialization.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2108 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/tools.py
+-rw-r--r--   0 zaber      (501) staff       (20)     9340 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/units.py
+-rw-r--r--   0 zaber      (501) staff       (20)       22 2023-08-08 20:12:08.000000 zaber_motion-4.2.5/zaber_motion/version.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-08-08 20:12:50.018939 zaber_motion-4.2.5/zaber_motion.egg-info/
+-rw-r--r--   0 zaber      (501) staff       (20)      808 2023-08-08 20:12:50.000000 zaber_motion-4.2.5/zaber_motion.egg-info/PKG-INFO
+-rw-r--r--   0 zaber      (501) staff       (20)     7890 2023-08-08 20:12:50.000000 zaber_motion-4.2.5/zaber_motion.egg-info/SOURCES.txt
+-rw-r--r--   0 zaber      (501) staff       (20)        1 2023-08-08 20:12:50.000000 zaber_motion-4.2.5/zaber_motion.egg-info/dependency_links.txt
+-rw-r--r--   0 zaber      (501) staff       (20)      239 2023-08-08 20:12:50.000000 zaber_motion-4.2.5/zaber_motion.egg-info/requires.txt
+-rw-r--r--   0 zaber      (501) staff       (20)       13 2023-08-08 20:12:50.000000 zaber_motion-4.2.5/zaber_motion.egg-info/top_level.txt
```

### Comparing `zaber_motion-4.2.4/LICENSE.txt` & `zaber_motion-4.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/PKG-INFO` & `zaber_motion-4.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaber_motion
-Version: 4.2.4
+Version: 4.2.5
 Summary: A library for communicating with Zaber devices
 Home-page: https://gitlab.com/ZaberTech/zaber-motion-lib
 Author: Zaber Technologies Inc.
 Author-email: contact@zaber.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `zaber_motion-4.2.4/setup.py` & `zaber_motion-4.2.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read_from_file(*filename):
     with open(path.join(*filename), 'r') as f:
         return f.read()
 
 
 setup(
     name='zaber_motion',
-    version='4.2.4',
+    version='4.2.5',
     packages=find_packages(exclude=["test*", "test_*", "*_test*"]),
     package_data={
         '': ['*.pyi', 'py.typed']
     },
     description='A library for communicating with Zaber devices',
     long_description=read_from_file('DESCRIPTION.md'),
     long_description_content_type="text/markdown",
@@ -32,12 +32,12 @@
         'License :: OSI Approved :: MIT License',
     ],
     keywords='',
     python_requires='>=3.8',
     install_requires=[
         'protobuf>=3.20.0,<4.22.0',
         'rx>=3.0.0',
-        'zaber_motion_bindings_windows==4.2.4;platform_system=="Windows"',
-        'zaber_motion_bindings_linux==4.2.4;platform_system=="Linux"',
-        'zaber_motion_bindings_darwin==4.2.4;platform_system=="Darwin"',
+        'zaber_motion_bindings_windows==4.2.5;platform_system=="Windows"',
+        'zaber_motion_bindings_linux==4.2.5;platform_system=="Linux"',
+        'zaber_motion_bindings_darwin==4.2.5;platform_system=="Darwin"',
     ],
 )
```

### Comparing `zaber_motion-4.2.4/test/test_integration.py` & `zaber_motion-4.2.5/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/__init__.py` & `zaber_motion-4.2.5/zaber_motion/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/__init__.py` & `zaber_motion-4.2.5/zaber_motion/ascii/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/alert_event.py` & `zaber_motion-4.2.5/zaber_motion/ascii/alert_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/all_axes.py` & `zaber_motion-4.2.5/zaber_motion/ascii/all_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/axis.py` & `zaber_motion-4.2.5/zaber_motion/ascii/axis.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/axis_identity.py` & `zaber_motion-4.2.5/zaber_motion/ascii/axis_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/axis_settings.py` & `zaber_motion-4.2.5/zaber_motion/ascii/axis_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/can_set_state_axis_response.py` & `zaber_motion-4.2.5/zaber_motion/ascii/can_set_state_axis_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/can_set_state_device_response.py` & `zaber_motion-4.2.5/zaber_motion/ascii/can_set_state_device_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/connection.py` & `zaber_motion-4.2.5/zaber_motion/ascii/connection.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/conversion_factor.py` & `zaber_motion-4.2.5/zaber_motion/ascii/conversion_factor.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/device.py` & `zaber_motion-4.2.5/zaber_motion/ascii/device.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/device_identity.py` & `zaber_motion-4.2.5/zaber_motion/ascii/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/device_io.py` & `zaber_motion-4.2.5/zaber_motion/ascii/device_io.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/device_io_info.py` & `zaber_motion-4.2.5/zaber_motion/ascii/device_io_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/device_settings.py` & `zaber_motion-4.2.5/zaber_motion/ascii/device_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/lockstep.py` & `zaber_motion-4.2.5/zaber_motion/ascii/lockstep.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/lockstep_axes.py` & `zaber_motion-4.2.5/zaber_motion/ascii/lockstep_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/oscilloscope.py` & `zaber_motion-4.2.5/zaber_motion/ascii/oscilloscope.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/oscilloscope_capture_properties.py` & `zaber_motion-4.2.5/zaber_motion/ascii/oscilloscope_capture_properties.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/oscilloscope_data.py` & `zaber_motion-4.2.5/zaber_motion/ascii/oscilloscope_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/paramset_info.py` & `zaber_motion-4.2.5/zaber_motion/ascii/paramset_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/pid_tuning.py` & `zaber_motion-4.2.5/zaber_motion/ascii/pid_tuning.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/process.py` & `zaber_motion-4.2.5/zaber_motion/ascii/process.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/process_controller.py` & `zaber_motion-4.2.5/zaber_motion/ascii/process_controller.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/process_controller_source.py` & `zaber_motion-4.2.5/zaber_motion/ascii/process_controller_source.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/pvt_axis_definition.py` & `zaber_motion-4.2.5/zaber_motion/ascii/pvt_axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/pvt_buffer.py` & `zaber_motion-4.2.5/zaber_motion/ascii/pvt_buffer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/pvt_sequence.py` & `zaber_motion-4.2.5/zaber_motion/ascii/pvt_sequence.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/response.py` & `zaber_motion-4.2.5/zaber_motion/ascii/response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/servo_tuner.py` & `zaber_motion-4.2.5/zaber_motion/ascii/servo_tuner.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/servo_tuning_param.py` & `zaber_motion-4.2.5/zaber_motion/ascii/servo_tuning_param.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/setting_constants.py` & `zaber_motion-4.2.5/zaber_motion/ascii/setting_constants.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/simple_tuning_param_definition.py` & `zaber_motion-4.2.5/zaber_motion/ascii/simple_tuning_param_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/storage.py` & `zaber_motion-4.2.5/zaber_motion/ascii/storage.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/stream.py` & `zaber_motion-4.2.5/zaber_motion/ascii/stream.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/stream_axis_definition.py` & `zaber_motion-4.2.5/zaber_motion/ascii/stream_axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/stream_buffer.py` & `zaber_motion-4.2.5/zaber_motion/ascii/stream_buffer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/transport.py` & `zaber_motion-4.2.5/zaber_motion/ascii/transport.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/unknown_response_event.py` & `zaber_motion-4.2.5/zaber_motion/ascii/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/warning_flags.py` & `zaber_motion-4.2.5/zaber_motion/ascii/warning_flags.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/ascii/warnings.py` & `zaber_motion-4.2.5/zaber_motion/ascii/warnings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/binary/__init__.py` & `zaber_motion-4.2.5/zaber_motion/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/binary/binary_settings.py` & `zaber_motion-4.2.5/zaber_motion/binary/binary_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/binary/command_code.py` & `zaber_motion-4.2.5/zaber_motion/binary/command_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/binary/connection.py` & `zaber_motion-4.2.5/zaber_motion/binary/connection.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/binary/device.py` & `zaber_motion-4.2.5/zaber_motion/binary/device.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/binary/device_identity.py` & `zaber_motion-4.2.5/zaber_motion/binary/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/binary/device_settings.py` & `zaber_motion-4.2.5/zaber_motion/binary/device_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/binary/error_code.py` & `zaber_motion-4.2.5/zaber_motion/binary/error_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/binary/message.py` & `zaber_motion-4.2.5/zaber_motion/binary/message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/binary/reply_only_event.py` & `zaber_motion-4.2.5/zaber_motion/binary/reply_only_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/binary/unknown_response_event.py` & `zaber_motion-4.2.5/zaber_motion/binary/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/bindings.py` & `zaber_motion-4.2.5/zaber_motion/bindings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/call.py` & `zaber_motion-4.2.5/zaber_motion/call.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/convert_exception.py` & `zaber_motion-4.2.5/zaber_motion/convert_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/events.py` & `zaber_motion-4.2.5/zaber_motion/events.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/__init__.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/binary_command_failed_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/binary_command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/binary_command_failed_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/binary_command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/command_failed_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/command_failed_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/command_too_long_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/command_too_long_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/command_too_long_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/command_too_long_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/device_address_conflict_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/device_address_conflict_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/device_address_conflict_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/device_address_conflict_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/device_db_failed_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/device_db_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/device_db_failed_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/device_db_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/g_code_execution_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/g_code_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/g_code_execution_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/g_code_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/g_code_syntax_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/g_code_syntax_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/g_code_syntax_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/g_code_syntax_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/invalid_packet_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/invalid_packet_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/invalid_packet_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/invalid_packet_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/invalid_pvt_point.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/invalid_pvt_point.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/invalid_response_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/invalid_response_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/invalid_response_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/invalid_response_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/movement_failed_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/movement_failed_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/movement_interrupted_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/movement_interrupted_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/pvt_execution_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/pvt_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/pvt_execution_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/pvt_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/pvt_movement_failed_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/pvt_movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/pvt_movement_failed_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/pvt_movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/pvt_movement_interrupted_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/pvt_movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/set_device_state_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/set_device_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/set_device_state_failed_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/set_device_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/set_peripheral_state_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/set_peripheral_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/set_peripheral_state_failed_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/set_peripheral_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/stream_execution_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/stream_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/stream_execution_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/stream_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/stream_movement_failed_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/stream_movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/stream_movement_failed_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/stream_movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/stream_movement_interrupted_exception.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/stream_movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py` & `zaber_motion-4.2.5/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/firmware_version.py` & `zaber_motion-4.2.5/zaber_motion/firmware_version.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/gcode/__init__.py` & `zaber_motion-4.2.5/zaber_motion/gcode/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/gcode/axis_definition.py` & `zaber_motion-4.2.5/zaber_motion/gcode/axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/gcode/axis_mapping.py` & `zaber_motion-4.2.5/zaber_motion/gcode/axis_mapping.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/gcode/axis_transformation.py` & `zaber_motion-4.2.5/zaber_motion/gcode/axis_transformation.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/gcode/device_definition.py` & `zaber_motion-4.2.5/zaber_motion/gcode/device_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/gcode/offline_translator.py` & `zaber_motion-4.2.5/zaber_motion/gcode/offline_translator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/gcode/translate_message.py` & `zaber_motion-4.2.5/zaber_motion/gcode/translate_message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/gcode/translate_result.py` & `zaber_motion-4.2.5/zaber_motion/gcode/translate_result.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/gcode/translator.py` & `zaber_motion-4.2.5/zaber_motion/gcode/translator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/gcode/translator_config.py` & `zaber_motion-4.2.5/zaber_motion/gcode/translator_config.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/library.py` & `zaber_motion-4.2.5/zaber_motion/library.py`

 * *Files 11% similar despite different names*

```diff
@@ -83,7 +83,23 @@
 
         Args:
             mode: Whether to turn internal mode on or off.
         """
         request = main_pb2.SetInternalModeRequest()
         request.mode = mode
         call_sync("library/set_internal_mode", request)
+
+    @staticmethod
+    def set_idle_polling_period(
+            period: int
+    ) -> None:
+        """
+        Sets the period between polling for IDLE during movements.
+        Caution: Setting the period too low may cause performance issues.
+
+        Args:
+            period: Period in milliseconds.
+                Negative value restores the default period.
+        """
+        request = main_pb2.IntRequest()
+        request.value = period
+        call_sync("library/set_idle_polling_period", request)
```

### Comparing `zaber_motion-4.2.4/zaber_motion/measurement.py` & `zaber_motion-4.2.5/zaber_motion/measurement.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/microscopy/objective_changer.py` & `zaber_motion-4.2.5/zaber_motion/microscopy/objective_changer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/protobufs/main_pb2.py` & `zaber_motion-4.2.5/zaber_motion/protobufs/main_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,458 +9,460 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14protobufs/main.proto\x12\x16zaber.motion.protobufs\"\x1a\n\x07Request\x12\x0f\n\x07request\x18\x01 \x01(\t\"\xb9\x01\n\x08Response\x12?\n\x08response\x18\x01 \x01(\x0e\x32-.zaber.motion.protobufs.Response.ResponseType\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"!\n\x0cResponseType\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x16\n\x05\x45vent\x12\r\n\x05\x65vent\x18\x01 \x01(\t\"\x0e\n\x0c\x45mptyRequest\"\x1d\n\x0c\x42oolResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\x1f\n\x0e\x44oubleResponse\x12\r\n\x05value\x18\x01 \x01(\x01\"%\n\x13\x44oubleArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"\x1c\n\x0bIntResponse\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1f\n\x0eStringResponse\x12\r\n\x05value\x18\x01 \x01(\t\"%\n\x13StringArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xdd\x01\n\x0c\x41xisIdentity\x12\x15\n\ris_peripheral\x18\x01 \x01(\x08\x12\x15\n\rperipheral_id\x18\x02 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x03 \x01(\t\x12@\n\taxis_type\x18\x04 \x01(\x0e\x32-.zaber.motion.protobufs.AxisIdentity.AxisType\x12\x13\n\x0bis_modified\x18\x05 \x01(\x08\"/\n\x08\x41xisType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\xcb\x01\n\x0e\x44\x65viceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\naxis_count\x18\x04 \x01(\x05\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x13\n\x0bis_modified\x18\x06 \x01(\x08\x12\x15\n\ris_integrated\x18\x07 \x01(\x08\">\n\x0f\x46irmwareVersion\x12\r\n\x05major\x18\x01 \x01(\x05\x12\r\n\x05minor\x18\x02 \x01(\x05\x12\r\n\x05\x62uild\x18\x03 \x01(\x05\"\x8a\x01\n\x0c\x44\x65viceIOInfo\x12\x1d\n\x15number_analog_outputs\x18\x02 \x01(\x05\x12\x1c\n\x14number_analog_inputs\x18\x03 \x01(\x05\x12\x1e\n\x16number_digital_outputs\x18\x04 \x01(\x05\x12\x1d\n\x15number_digital_inputs\x18\x05 \x01(\x05\";\n\x0bMeasurement\x12\r\n\x05value\x18\x01 \x01(\x01\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\x0f\n\x07is_null\x18\x03 \x01(\x08\">\n\x14StreamAxisDefinition\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x11\n\taxis_type\x18\x02 \x01(\x05\"<\n\x1aInvalidPacketExceptionData\x12\x0e\n\x06packet\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\">\n\"DeviceAddressConflictExceptionData\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"b\n MovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"J\n&StreamMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"G\n#PvtMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"]\n\x1bMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"E\n!StreamMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1ePvtMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1cStreamExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"\x80\x01\n\x19PvtExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12?\n\x0einvalid_points\x18\x03 \x03(\x0b\x32\'.zaber.motion.protobufs.InvalidPvtPoint\"/\n\x0fInvalidPvtPoint\x12\r\n\x05index\x18\x01 \x01(\x05\x12\r\n\x05point\x18\x02 \x01(\t\"0\n\x1cInvalidResponseExceptionData\x12\x10\n\x08response\x18\x01 \x01(\t\"\xb7\x01\n\x1a\x43ommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\t\x12\x12\n\nreply_flag\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x04 \x01(\t\x12\x16\n\x0e\x64\x65vice_address\x18\x05 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x06 \x01(\x05\x12\n\n\x02id\x18\x07 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x08 \x01(\t\"9\n BinaryCommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\x05\"\x89\x01\n\x1fSetPeripheralStateExceptionData\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x10\n\x08settings\x18\x02 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x03 \x01(\t\x12\x0f\n\x07storage\x18\x04 \x03(\t\x12\x18\n\x10stored_positions\x18\x05 \x03(\t\"\xfd\x01\n\x1bSetDeviceStateExceptionData\x12L\n\x0bperipherals\x18\x02 \x03(\x0b\x32\x37.zaber.motion.protobufs.SetPeripheralStateExceptionData\x12\x10\n\x08settings\x18\x03 \x03(\t\x12\x16\n\x0estream_buffers\x18\x04 \x03(\t\x12\x10\n\x08triggers\x18\x05 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x06 \x01(\t\x12\x0f\n\x07storage\x18\x07 \x03(\t\x12\x18\n\x10stored_positions\x18\x08 \x03(\t\x12\x13\n\x0bpvt_buffers\x18\t \x03(\t\"g\n\x1b\x43ommandTooLongExceptionData\x12\x0b\n\x03\x66it\x18\x01 \x01(\t\x12\x11\n\tremainder\x18\x02 \x01(\t\x12\x13\n\x0bpacket_size\x18\x03 \x01(\x05\x12\x13\n\x0bpackets_max\x18\x04 \x01(\x05\"V\n\x0bTestRequest\x12\x14\n\x0creturn_error\x18\x01 \x01(\x08\x12\x11\n\tdata_ping\x18\x02 \x01(\t\x12\x1e\n\x16return_error_with_data\x18\x03 \x01(\x08\"!\n\x0cTestResponse\x12\x11\n\tdata_pong\x18\x01 \x01(\t\"%\n\x10TestResponseLong\x12\x11\n\tdata_pong\x18\x01 \x03(\t\"\x19\n\tTestEvent\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"-\n\x1cToolsListSerialPortsResponse\x12\r\n\x05ports\x18\x01 \x03(\t\"&\n\x16SetInternalModeRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x08\"I\n\x18SetDeviceDbSourceRequest\x12\x13\n\x0bsource_type\x18\x01 \x01(\x05\x12\x18\n\x10url_or_file_path\x18\x02 \x01(\t\"G\n\x1aToggleDeviceDbStoreRequest\x12\x11\n\ttoggle_on\x18\x01 \x01(\x08\x12\x16\n\x0estore_location\x18\x02 \x01(\t\"+\n\x1b\x44\x65viceDbFailedExceptionData\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xa7\x02\n\x14OpenInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x11\n\ttransport\x18\x06 \x01(\x05\x12 \n\x18reject_routed_connection\x18\x07 \x01(\x08\x12\x10\n\x08\x63loud_id\x18\x08 \x01(\t\x12\x17\n\x0f\x63onnection_name\x18\t \x01(\t\x12\r\n\x05realm\x18\n \x01(\t\x12\r\n\x05token\x18\x0b \x01(\t\x12\x0b\n\x03\x61pi\x18\x0c \x01(\t\"-\n\x15OpenInterfaceResponse\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"-\n\x15InterfaceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"C\n\x1aSetInterfaceTimeoutRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\"N\n\"SetInterfaceChecksumEnabledRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\"F\n\x10\x41xisEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\"\x83\x01\n\x15GenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x05\"\xc8\x01\n\x16GenericCommandResponse\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"e\n GenericCommandResponseCollection\x12\x41\n\tresponses\x18\x02 \x03(\x0b\x32..zaber.motion.protobufs.GenericCommandResponse\"\xdc\x01\n\x14UnknownResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"\x83\x01\n\nAlertEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\t\"t\n\x11\x44isconnectedEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"~\n\x15\x44\x65viceIdentifyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12?\n\x0e\x61ssume_version\x18\x03 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\"D\n\x15\x44\x65viceRenumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x15\n\rfirst_address\x18\x02 \x01(\x05\"\xba\x01\n\x13\x44\x65viceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\x12\x44\n\x04type\x18\x03 \x01(\x0e\x32\x36.zaber.motion.protobufs.DeviceDetectRequest.DeviceType\"-\n\nDeviceType\x12\x07\n\x03\x41NY\x10\x00\x12\x16\n\x12PROCESS_CONTROLLER\x10\x01\"\'\n\x14\x44\x65viceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"`\n\x11\x44\x65viceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"n\n\x1a\x44\x65viceWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"\xd0\x02\n\x11\x44\x65viceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12@\n\x04type\x18\x05 \x01(\x0e\x32\x32.zaber.motion.protobufs.DeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\x10\n\x08velocity\x18\x08 \x01(\x01\x12\x15\n\rvelocity_unit\x18\t \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\n \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0b \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"`\n\x11\x44\x65viceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"C\n\x12\x44\x65viceOnAllRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"/\n\x13\x44\x65viceOnAllResponse\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"]\n\x18\x44\x65viceGetWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05\x63lear\x18\x04 \x01(\x08\"*\n\x19\x44\x65viceGetWarningsResponse\x12\r\n\x05\x66lags\x18\x01 \x03(\t\"x\n\x1aWaitToClearWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07timeout\x18\x04 \x01(\x01\x12\x15\n\rwarning_flags\x18\x05 \x03(\t\"Z\n\x1c\x44\x65viceGetAllDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\"/\n\x1d\x44\x65viceGetAllDigitalIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x08\"Y\n\x1b\x44\x65viceGetAllAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\".\n\x1c\x44\x65viceGetAllAnalogIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"o\n\x19\x44\x65viceGetDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"n\n\x18\x44\x65viceGetAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"Y\n!DeviceSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x08\"X\n DeviceSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x01\"l\n\x1d\x44\x65viceSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x08\"k\n\x1c\x44\x65viceSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\"6\n\x13SetLogOutputRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x05\x12\x11\n\tfile_path\x18\x02 \x01(\t\"l\n\x17\x44\x65viceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x94\x01\n\x1b\x44\x65viceConvertSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\r\n\x05value\x18\x06 \x01(\x01\x12\x13\n\x0b\x66rom_native\x18\x07 \x01(\x08\"{\n\x17\x44\x65viceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"p\n\x1a\x44\x65viceSetSettingStrRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\"\x9e\x01\n\x15PrepareCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x18\n\x10\x63ommand_template\x18\x04 \x01(\t\x12\x37\n\nparameters\x18\x05 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"M\n\x14WaitToRespondRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\"f\n\x15LockstepEnableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x04 \x03(\x05\"r\n\x16LockstepDisableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"\xe1\x02\n\x13LockstepMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12\x42\n\x04type\x18\x05 \x01(\x0e\x32\x34.zaber.motion.protobufs.LockstepMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x08 \x01(\t\x12\x10\n\x08velocity\x18\t \x01(\x01\x12\x15\n\rvelocity_unit\x18\n \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\x0b \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0c \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"}\n\x1cLockstepWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"W\n\x14LockstepEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\"N\n\x0cLockstepAxes\x12\x0e\n\x06\x61xis_1\x18\x01 \x01(\x05\x12\x0e\n\x06\x61xis_2\x18\x02 \x01(\x05\x12\x0e\n\x06\x61xis_3\x18\x03 \x01(\x05\x12\x0e\n\x06\x61xis_4\x18\x04 \x01(\x05\".\n\x1eLockstepGetAxisNumbersResponse\x12\x0c\n\x04\x61xes\x18\x01 \x03(\x05\"c\n\x12LockstepGetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x86\x01\n\x12LockstepSetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\x12\n\naxis_index\x18\x06 \x01(\x05\"k\n$OscilloscopeAddSettingChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\"l\n\x1fOscilloscopeAddIoChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07io_type\x18\x03 \x01(\x05\x12\x12\n\nio_channel\x18\x04 \x01(\x05\"k\n\x1cOscilloscopeStartStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\r\n\x05start\x18\x03 \x01(\x08\x12\x16\n\x0e\x63\x61pture_length\x18\x04 \x01(\x05\",\n\x18OscilloscopeReadResponse\x12\x10\n\x08\x64\x61ta_ids\x18\x01 \x03(\x05\"-\n\x1aOscilloscopeDataIdentifier\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\"\x7f\n\x1dOscilloscopeCaptureProperties\x12\x13\n\x0b\x64\x61ta_source\x18\x01 \x01(\x05\x12\x0f\n\x07setting\x18\x02 \x01(\t\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0f\n\x07io_type\x18\x04 \x01(\x05\x12\x12\n\nio_channel\x18\x05 \x01(\x05\";\n\x1aOscilloscopeDataGetRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\"T\n$OscilloscopeDataGetSampleTimeRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\"2\n\"OscilloscopeDataGetSamplesResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x01\"l\n\x16StreamSetupLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04\x61xes\x18\x05 \x03(\x05\"\xa3\x01\n\x1fStreamSetupLiveCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04\x61xes\x18\x05 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\x98\x01\n\x17StreamSetupStoreRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x07 \x03(\x05\"\xcf\x01\n StreamSetupStoreCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12:\n\x04\x61xes\x18\x07 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\xab\x01\n$StreamSetupStoreArbitraryAxesRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x12\n\naxes_count\x18\x07 \x01(\x05\"\x84\x01\n\x11StreamCallRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\"\xd1\x02\n\x0fPvtPointRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04type\x18\x05 \x01(\x0e\x32,.zaber.motion.protobufs.PvtPointRequest.Type\x12\x36\n\tpositions\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x37\n\nvelocities\x18\x07 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x31\n\x04time\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x85\x02\n\x11StreamLineRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12<\n\x04type\x18\x05 \x01(\x0e\x32..zaber.motion.protobufs.StreamLineRequest.Type\x12\x35\n\x08\x65ndpoint\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x07 \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xf5\x03\n\x10StreamArcRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12;\n\x04type\x18\x05 \x01(\x0e\x32-.zaber.motion.protobufs.StreamArcRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_x\x18\t \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_y\x18\n \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x0b \x03(\x05\x12\x35\n\x08\x65ndpoint\x18\x0c \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xdc\x02\n\x13StreamCircleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12>\n\x04type\x18\x05 \x01(\x0e\x32\x30.zaber.motion.protobufs.StreamCircleRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\t \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x8c\x01\n\x1dStreamWaitDigitalInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x9e\x01\n\x1cStreamWaitAnalogInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\x11\n\tcondition\x18\x06 \x01(\t\x12\r\n\x05value\x18\x07 \x01(\x01\"\x8c\x01\n\x1dStreamSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x8b\x01\n\x1cStreamSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x01\"\x80\x01\n StreamToggleDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\"y\n!StreamSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x08\"x\n StreamSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x01\"u\n\x11StreamWaitRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04time\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n\x1aStreamWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x1c\n\x14throw_error_on_fault\x18\x05 \x01(\x08\"Z\n\x12StreamEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"S\n\x15StreamGetAxesResponse\x12:\n\x04\x61xes\x18\x01 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"n\n\x18StreamGetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x81\x01\n\x18StreamSetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x05 \x01(\x08\x12\x11\n\tmax_speed\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\"\x7f\n)StreamGetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa4\x01\n)StreamSetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12#\n\x1bmax_tangential_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n*StreamGetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa6\x01\n*StreamSetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12$\n\x1cmax_centripetal_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"e\n\x1dStreamBufferGetContentRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"6\n\x1eStreamBufferGetContentResponse\x12\x14\n\x0c\x62uffer_lines\x18\x01 \x03(\t\"`\n\x18StreamBufferEraseRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"t\n\x1bStreamGenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0f\n\x07\x63ommand\x18\x05 \x01(\t\"w\n StreamGenericCommandBatchRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\r\n\x05\x62\x61tch\x18\x05 \x03(\t\"c\n\x14\x42inaryReplyOnlyEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\xbb\x01\n\x1aOpenBinaryInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x17\n\x0fuse_message_ids\x18\x06 \x01(\x08\"i\n\x1aUnknownBinaryResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\x82\x01\n\x14GenericBinaryRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x01\"F\n\rBinaryMessage\x12\x16\n\x0e\x64\x65vice_address\x18\x01 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x05\"R\n\x17\x42inaryMessageCollection\x12\x37\n\x08messages\x18\x02 \x03(\x0b\x32%.zaber.motion.protobufs.BinaryMessage\":\n\x12\x44\x65viceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\"\xd9\x02\n\x14\x42inaryDeviceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x15\n\ris_peripheral\x18\x06 \x01(\x08\x12\x15\n\rperipheral_id\x18\x07 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x08 \x01(\t\x12L\n\x0b\x64\x65vice_type\x18\t \x01(\x0e\x32\x37.zaber.motion.protobufs.BinaryDeviceIdentity.DeviceType\"1\n\nDeviceType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\x99\x01\n\x1d\x42inaryGenericWithUnitsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x01\x12\x11\n\tfrom_unit\x18\x05 \x01(\t\x12\x0f\n\x07to_unit\x18\x06 \x01(\t\x12\x0f\n\x07timeout\x18\x07 \x01(\x01\"^\n\x17\x42inaryDeviceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\xda\x01\n\x17\x42inaryDeviceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x46\n\x04type\x18\x04 \x01(\x0e\x32\x38.zaber.motion.protobufs.BinaryDeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"%\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\"^\n\x17\x42inaryDeviceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"K\n\x19\x42inaryDeviceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"-\n\x1a\x42inaryDeviceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"d\n\x1d\x42inaryDeviceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"s\n\x1d\x42inaryDeviceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"2\n\x1a\x43ustomInterfaceReadRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"D\n\x1b\x43ustomInterfaceWriteRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"3\n\x1b\x43ustomInterfaceOpenResponse\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"J\n\x1b\x43ustomInterfaceCloseRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"W\n\x12\x43\x61nSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\"=\n\x17\x43\x61nSetStateAxisResponse\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"p\n\x19\x43\x61nSetStateDeviceResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x44\n\x0b\x61xis_errors\x18\x02 \x03(\x0b\x32/.zaber.motion.protobufs.CanSetStateAxisResponse\"i\n\x0fSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65vice_only\x18\x05 \x01(\x08\"Z\n\x12ServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\"/\n\x10ServoTuningParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"g\n\x0cParamsetInfo\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x05\x12\x38\n\x06params\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"\x9e\x01\n\x15SetServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12?\n\rtuning_params\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"n\n\x0cLoadParamset\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x13\n\x0bto_paramset\x18\x04 \x01(\x05\x12\x15\n\rfrom_paramset\x18\x05 \x01(\x05\"\x8d\x01\n\x18SetServoTuningPIDRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\t\n\x01p\x18\x05 \x01(\x01\x12\t\n\x01i\x18\x06 \x01(\x01\x12\t\n\x01\x64\x18\x07 \x01(\x01\x12\n\n\x02\x66\x63\x18\x08 \x01(\x01\"W\n\tPidTuning\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\t\n\x01p\x18\x03 \x01(\x01\x12\t\n\x01i\x18\x04 \x01(\x01\x12\t\n\x01\x64\x18\x05 \x01(\x01\x12\n\n\x02\x66\x63\x18\x06 \x01(\x01\"\xc2\x01\n\x0fSetSimpleTuning\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\x15\n\rcarriage_mass\x18\x05 \x01(\x01\x12\x11\n\tload_mass\x18\x06 \x01(\x01\x12?\n\rtuning_params\x18\x07 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"d\n\x1bSimpleTuningParamDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tmin_label\x18\x02 \x01(\t\x12\x11\n\tmax_label\x18\x03 \x01(\t\x12\x11\n\tdata_type\x18\x04 \x01(\t\"m\n&GetSimpleTuningParamDefinitionResponse\x12\x43\n\x06params\x18\x01 \x03(\x0b\x32\x33.zaber.motion.protobufs.SimpleTuningParamDefinition\"\x95\x01\n\x17TranslatorCreateRequest\x12@\n\ndefinition\x18\x01 \x01(\x0b\x32,.zaber.motion.protobufs.TranslatorDefinition\x12\x38\n\x06\x63onfig\x18\x02 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"1\n\x18TranslatorCreateResponse\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"O\n\x18TranslatorAxisDefinition\x12\x15\n\rperipheral_id\x18\x01 \x01(\x05\x12\x1c\n\x14microstep_resolution\x18\x02 \x01(\x05\"\xa1\x01\n\x14TranslatorDefinition\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12>\n\x04\x61xes\x18\x02 \x03(\x0b\x32\x30.zaber.motion.protobufs.TranslatorAxisDefinition\x12\x36\n\tmax_speed\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\xac\x01\n\x10TranslatorConfig\x12\x44\n\raxis_mappings\x18\x01 \x03(\x0b\x32-.zaber.motion.protobufs.TranslatorAxisMapping\x12R\n\x14\x61xis_transformations\x18\x02 \x03(\x0b\x32\x34.zaber.motion.protobufs.TranslatorAxisTransformation\"@\n\x15TranslatorAxisMapping\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x12\n\naxis_index\x18\x02 \x01(\x05\"~\n\x1cTranslatorAxisTransformation\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x0f\n\x07scaling\x18\x02 \x01(\x01\x12\x38\n\x0btranslation\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"B\n\x1aTranslatorTranslateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\r\n\x05\x62lock\x18\x02 \x01(\t\"I\n\x10TranslateMessage\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x12\n\nfrom_block\x18\x02 \x01(\x05\x12\x10\n\x08to_block\x18\x03 \x01(\x05\"k\n\x1bTranslatorTranslateResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\x12:\n\x08warnings\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.TranslateMessage\"@\n\x18GCodeSyntaxExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"C\n\x1bGCodeExecutionExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"L\n\x1aTranslatorFlushLiveRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"+\n\x17TranslatorFlushResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\"\x90\x01\n\x1bTranslatorCreateLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"\x91\x01\n!TranslatorCreateFromDeviceRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x03 \x03(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"/\n\x16TranslatorEmptyRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"^\n TranslatorSetTraverseRateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x15\n\rtraverse_rate\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"g\n TranslatorSetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x10\n\x08position\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"U\n TranslatorGetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x0c\n\x04unit\x18\x03 \x01(\t\"n\n\x1eTranslatorGetAxisOffsetRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x19\n\x11\x63oordinate_system\x18\x02 \x01(\t\x12\x0c\n\x04\x61xis\x18\x03 \x01(\t\x12\x0c\n\x04unit\x18\x04 \x01(\t\"R\n$TranslatorSetFeedRateOverrideRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x13\n\x0b\x63oefficient\x18\x02 \x01(\x01\"y\n\x17\x44\x65viceSetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\x12\x0e\n\x06\x65ncode\x18\x06 \x01(\x08\"j\n\x17\x44\x65viceGetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\x0e\n\x06\x64\x65\x63ode\x18\x05 \x01(\x08\"o\n\x1d\x44\x65viceSetStorageNumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\"m\n\x1b\x44\x65viceSetStorageBoolRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x08\"W\n\x14\x44\x65viceStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\"b\n\x1c\x44\x65viceStorageListKeysRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0e\n\x06prefix\x18\x04 \x01(\t\"\xa1\x01\n\x1f\x44\x65viceSetUnitConversionsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12=\n\x0b\x63onversions\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ConversionFactor\"@\n\x10\x43onversionFactor\x12\x0f\n\x07setting\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"^\n\x17ObjectiveChangerRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\"?\n\x1eObjectiveChangerCreateResponse\x12\x0e\n\x06turret\x18\x02 \x01(\x05\x12\r\n\x05\x66ocus\x18\x03 \x01(\x05\"\xb2\x01\n\x1dObjectiveChangerChangeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\x12\x11\n\tobjective\x18\x04 \x01(\x05\x12\x39\n\x0c\x66ocus_offset\x18\x05 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"3\n\"ObjectiveChangerGetCurrentResponse\x12\r\n\x05value\x18\x01 \x01(\x05\"]\n\tProcessOn\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\n\n\x02on\x18\x04 \x01(\x08\x12\x10\n\x08\x64uration\x18\x05 \x01(\x01\"7\n\x17ProcessControllerSource\x12\x0e\n\x06sensor\x18\x01 \x01(\x05\x12\x0c\n\x04port\x18\x02 \x01(\x05\"\x91\x01\n\x1aSetProcessControllerSource\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12?\n\x06source\x18\x04 \x01(\x0b\x32/.zaber.motion.protobufs.ProcessControllerSource*-\n\x0bMessageType\x12\t\n\x05REPLY\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\t\n\x05\x41LERT\x10\x02*\xc0\t\n\x06\x45rrors\x12\x13\n\x0fREQUEST_TIMEOUT\x10\x00\x12\x15\n\x11\x43ONNECTION_CLOSED\x10\x01\x12\x14\n\x10INVALID_ARGUMENT\x10\x02\x12\x16\n\x12OUT_OF_REQUEST_IDS\x10\x03\x12\x12\n\x0eINVALID_PACKET\x10\x04\x12\x15\n\x11\x43ONNECTION_FAILED\x10\x05\x12\x13\n\x0fUNKNOWN_REQUEST\x10\x06\x12\x12\n\x0e\x43OMMAND_FAILED\x10\x07\x12\x14\n\x10\x44\x45VICE_DB_FAILED\x10\x08\x12\x10\n\x0cINVALID_DATA\x10\t\x12\x19\n\x15\x44\x45VICE_NOT_IDENTIFIED\x10\n\x12\x15\n\x11\x43ONVERSION_FAILED\x10\x0b\x12\x1b\n\x17\x44\x45VICE_ADDRESS_CONFLICT\x10\x0c\x12\x13\n\x0fNO_DEVICE_FOUND\x10\r\x12\x18\n\x14MOVEMENT_INTERRUPTED\x10\x0e\x12\x13\n\x0fMOVEMENT_FAILED\x10\x0f\x12\r\n\tIO_FAILED\x10\x10\x12\x14\n\x10INVALID_RESPONSE\x10\x11\x12\x11\n\rNOT_SUPPORTED\x10\x12\x12\x11\n\rDEVICE_FAILED\x10\x13\x12\r\n\tOS_FAILED\x10\x14\x12\x12\n\x0eINTERNAL_ERROR\x10\x16\x12\x19\n\x15\x42INARY_COMMAND_FAILED\x10\x18\x12\x15\n\x11\x43OMMAND_PREEMPTED\x10\x19\x12\x18\n\x14LOCKSTEP_NOT_ENABLED\x10\x1a\x12\x14\n\x10LOCKSTEP_ENABLED\x10\x1b\x12\x1b\n\x17IO_CHANNEL_OUT_OF_RANGE\x10\x1c\x12\x15\n\x11SETTING_NOT_FOUND\x10\x1d\x12\x0f\n\x0bSTREAM_MODE\x10\x1e\x12\x14\n\x10STREAM_EXECUTION\x10\x1f\x12\x1a\n\x16STREAM_MOVEMENT_FAILED\x10 \x12\x17\n\x13STREAM_SETUP_FAILED\x10!\x12\x0f\n\x0b\x44\x45VICE_BUSY\x10\"\x12\x1f\n\x1bSTREAM_MOVEMENT_INTERRUPTED\x10#\x12\x16\n\x12INVALID_PARK_STATE\x10$\x12\x14\n\x10SERIAL_PORT_BUSY\x10%\x12\x1a\n\x16TRANSPORT_ALREADY_USED\x10&\x12\x1f\n\x1bSET_PERIPHERAL_STATE_FAILED\x10\'\x12\x1b\n\x17SET_DEVICE_STATE_FAILED\x10(\x12\x11\n\rG_CODE_SYNTAX\x10)\x12\x14\n\x10G_CODE_EXECUTION\x10*\x12\x15\n\x11INVALID_OPERATION\x10+\x12\x14\n\x10\x43OMMAND_TOO_LONG\x10,\x12\x14\n\x10NO_VALUE_FOR_KEY\x10-\x12\x1b\n\x17\x44\x45VICE_DETECTION_FAILED\x10.\x12\x0b\n\x07TIMEOUT\x10/\x12\x0c\n\x08PVT_MODE\x10\x30\x12\x11\n\rPVT_EXECUTION\x10\x31\x12\x14\n\x10PVT_SETUP_FAILED\x10\x32\x12\x17\n\x13PVT_MOVEMENT_FAILED\x10\x33\x12\x1c\n\x18PVT_MOVEMENT_INTERRUPTED\x10\x34\x12\x15\n\x11PVT_DISCONTINUITY\x10\x35\x12\x18\n\x14STREAM_DISCONTINUITY\x10\x36*Q\n\rInterfaceType\x12\x0f\n\x0bSERIAL_PORT\x10\x00\x12\x07\n\x03TCP\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\x07\n\x03IOT\x10\x03\x12\x11\n\rNETWORK_SHARE\x10\x04\x42$Z\"./protobufs;zaber_motion_protobufsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14protobufs/main.proto\x12\x16zaber.motion.protobufs\"\x1a\n\x07Request\x12\x0f\n\x07request\x18\x01 \x01(\t\"\xb9\x01\n\x08Response\x12?\n\x08response\x18\x01 \x01(\x0e\x32-.zaber.motion.protobufs.Response.ResponseType\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"!\n\x0cResponseType\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x16\n\x05\x45vent\x12\r\n\x05\x65vent\x18\x01 \x01(\t\"\x0e\n\x0c\x45mptyRequest\"\x1b\n\nIntRequest\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1d\n\x0c\x42oolResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\x1f\n\x0e\x44oubleResponse\x12\r\n\x05value\x18\x01 \x01(\x01\"%\n\x13\x44oubleArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"\x1c\n\x0bIntResponse\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1f\n\x0eStringResponse\x12\r\n\x05value\x18\x01 \x01(\t\"%\n\x13StringArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xdd\x01\n\x0c\x41xisIdentity\x12\x15\n\ris_peripheral\x18\x01 \x01(\x08\x12\x15\n\rperipheral_id\x18\x02 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x03 \x01(\t\x12@\n\taxis_type\x18\x04 \x01(\x0e\x32-.zaber.motion.protobufs.AxisIdentity.AxisType\x12\x13\n\x0bis_modified\x18\x05 \x01(\x08\"/\n\x08\x41xisType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\xcb\x01\n\x0e\x44\x65viceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\naxis_count\x18\x04 \x01(\x05\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x13\n\x0bis_modified\x18\x06 \x01(\x08\x12\x15\n\ris_integrated\x18\x07 \x01(\x08\">\n\x0f\x46irmwareVersion\x12\r\n\x05major\x18\x01 \x01(\x05\x12\r\n\x05minor\x18\x02 \x01(\x05\x12\r\n\x05\x62uild\x18\x03 \x01(\x05\"\x8a\x01\n\x0c\x44\x65viceIOInfo\x12\x1d\n\x15number_analog_outputs\x18\x02 \x01(\x05\x12\x1c\n\x14number_analog_inputs\x18\x03 \x01(\x05\x12\x1e\n\x16number_digital_outputs\x18\x04 \x01(\x05\x12\x1d\n\x15number_digital_inputs\x18\x05 \x01(\x05\";\n\x0bMeasurement\x12\r\n\x05value\x18\x01 \x01(\x01\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\x0f\n\x07is_null\x18\x03 \x01(\x08\">\n\x14StreamAxisDefinition\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x11\n\taxis_type\x18\x02 \x01(\x05\"<\n\x1aInvalidPacketExceptionData\x12\x0e\n\x06packet\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\">\n\"DeviceAddressConflictExceptionData\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"b\n MovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"J\n&StreamMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"G\n#PvtMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"]\n\x1bMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"E\n!StreamMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1ePvtMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1cStreamExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"\x80\x01\n\x19PvtExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12?\n\x0einvalid_points\x18\x03 \x03(\x0b\x32\'.zaber.motion.protobufs.InvalidPvtPoint\"/\n\x0fInvalidPvtPoint\x12\r\n\x05index\x18\x01 \x01(\x05\x12\r\n\x05point\x18\x02 \x01(\t\"0\n\x1cInvalidResponseExceptionData\x12\x10\n\x08response\x18\x01 \x01(\t\"\xb7\x01\n\x1a\x43ommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\t\x12\x12\n\nreply_flag\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x04 \x01(\t\x12\x16\n\x0e\x64\x65vice_address\x18\x05 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x06 \x01(\x05\x12\n\n\x02id\x18\x07 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x08 \x01(\t\"9\n BinaryCommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\x05\"\x89\x01\n\x1fSetPeripheralStateExceptionData\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x10\n\x08settings\x18\x02 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x03 \x01(\t\x12\x0f\n\x07storage\x18\x04 \x03(\t\x12\x18\n\x10stored_positions\x18\x05 \x03(\t\"\xfd\x01\n\x1bSetDeviceStateExceptionData\x12L\n\x0bperipherals\x18\x02 \x03(\x0b\x32\x37.zaber.motion.protobufs.SetPeripheralStateExceptionData\x12\x10\n\x08settings\x18\x03 \x03(\t\x12\x16\n\x0estream_buffers\x18\x04 \x03(\t\x12\x10\n\x08triggers\x18\x05 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x06 \x01(\t\x12\x0f\n\x07storage\x18\x07 \x03(\t\x12\x18\n\x10stored_positions\x18\x08 \x03(\t\x12\x13\n\x0bpvt_buffers\x18\t \x03(\t\"g\n\x1b\x43ommandTooLongExceptionData\x12\x0b\n\x03\x66it\x18\x01 \x01(\t\x12\x11\n\tremainder\x18\x02 \x01(\t\x12\x13\n\x0bpacket_size\x18\x03 \x01(\x05\x12\x13\n\x0bpackets_max\x18\x04 \x01(\x05\"V\n\x0bTestRequest\x12\x14\n\x0creturn_error\x18\x01 \x01(\x08\x12\x11\n\tdata_ping\x18\x02 \x01(\t\x12\x1e\n\x16return_error_with_data\x18\x03 \x01(\x08\"!\n\x0cTestResponse\x12\x11\n\tdata_pong\x18\x01 \x01(\t\"%\n\x10TestResponseLong\x12\x11\n\tdata_pong\x18\x01 \x03(\t\"\x19\n\tTestEvent\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"-\n\x1cToolsListSerialPortsResponse\x12\r\n\x05ports\x18\x01 \x03(\t\"&\n\x16SetInternalModeRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x08\"I\n\x18SetDeviceDbSourceRequest\x12\x13\n\x0bsource_type\x18\x01 \x01(\x05\x12\x18\n\x10url_or_file_path\x18\x02 \x01(\t\"G\n\x1aToggleDeviceDbStoreRequest\x12\x11\n\ttoggle_on\x18\x01 \x01(\x08\x12\x16\n\x0estore_location\x18\x02 \x01(\t\"+\n\x1b\x44\x65viceDbFailedExceptionData\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xa7\x02\n\x14OpenInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x11\n\ttransport\x18\x06 \x01(\x05\x12 \n\x18reject_routed_connection\x18\x07 \x01(\x08\x12\x10\n\x08\x63loud_id\x18\x08 \x01(\t\x12\x17\n\x0f\x63onnection_name\x18\t \x01(\t\x12\r\n\x05realm\x18\n \x01(\t\x12\r\n\x05token\x18\x0b \x01(\t\x12\x0b\n\x03\x61pi\x18\x0c \x01(\t\"-\n\x15OpenInterfaceResponse\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"-\n\x15InterfaceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"C\n\x1aSetInterfaceTimeoutRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\"N\n\"SetInterfaceChecksumEnabledRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\"F\n\x10\x41xisEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\"\x83\x01\n\x15GenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x05\"\xc8\x01\n\x16GenericCommandResponse\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"e\n GenericCommandResponseCollection\x12\x41\n\tresponses\x18\x02 \x03(\x0b\x32..zaber.motion.protobufs.GenericCommandResponse\"\xdc\x01\n\x14UnknownResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"\x83\x01\n\nAlertEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\t\"t\n\x11\x44isconnectedEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"~\n\x15\x44\x65viceIdentifyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12?\n\x0e\x61ssume_version\x18\x03 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\"D\n\x15\x44\x65viceRenumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x15\n\rfirst_address\x18\x02 \x01(\x05\"\xba\x01\n\x13\x44\x65viceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\x12\x44\n\x04type\x18\x03 \x01(\x0e\x32\x36.zaber.motion.protobufs.DeviceDetectRequest.DeviceType\"-\n\nDeviceType\x12\x07\n\x03\x41NY\x10\x00\x12\x16\n\x12PROCESS_CONTROLLER\x10\x01\"\'\n\x14\x44\x65viceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"`\n\x11\x44\x65viceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"n\n\x1a\x44\x65viceWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"\xd0\x02\n\x11\x44\x65viceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12@\n\x04type\x18\x05 \x01(\x0e\x32\x32.zaber.motion.protobufs.DeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\x10\n\x08velocity\x18\x08 \x01(\x01\x12\x15\n\rvelocity_unit\x18\t \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\n \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0b \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"`\n\x11\x44\x65viceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"C\n\x12\x44\x65viceOnAllRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"/\n\x13\x44\x65viceOnAllResponse\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"]\n\x18\x44\x65viceGetWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05\x63lear\x18\x04 \x01(\x08\"*\n\x19\x44\x65viceGetWarningsResponse\x12\r\n\x05\x66lags\x18\x01 \x03(\t\"x\n\x1aWaitToClearWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07timeout\x18\x04 \x01(\x01\x12\x15\n\rwarning_flags\x18\x05 \x03(\t\"Z\n\x1c\x44\x65viceGetAllDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\"/\n\x1d\x44\x65viceGetAllDigitalIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x08\"Y\n\x1b\x44\x65viceGetAllAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\".\n\x1c\x44\x65viceGetAllAnalogIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"o\n\x19\x44\x65viceGetDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"n\n\x18\x44\x65viceGetAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"Y\n!DeviceSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x08\"X\n DeviceSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x01\"l\n\x1d\x44\x65viceSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x08\"k\n\x1c\x44\x65viceSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\"6\n\x13SetLogOutputRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x05\x12\x11\n\tfile_path\x18\x02 \x01(\t\"l\n\x17\x44\x65viceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x94\x01\n\x1b\x44\x65viceConvertSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\r\n\x05value\x18\x06 \x01(\x01\x12\x13\n\x0b\x66rom_native\x18\x07 \x01(\x08\"{\n\x17\x44\x65viceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"p\n\x1a\x44\x65viceSetSettingStrRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\"\x9e\x01\n\x15PrepareCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x18\n\x10\x63ommand_template\x18\x04 \x01(\t\x12\x37\n\nparameters\x18\x05 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"M\n\x14WaitToRespondRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\"f\n\x15LockstepEnableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x04 \x03(\x05\"r\n\x16LockstepDisableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"\xe1\x02\n\x13LockstepMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12\x42\n\x04type\x18\x05 \x01(\x0e\x32\x34.zaber.motion.protobufs.LockstepMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x08 \x01(\t\x12\x10\n\x08velocity\x18\t \x01(\x01\x12\x15\n\rvelocity_unit\x18\n \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\x0b \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0c \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"}\n\x1cLockstepWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"W\n\x14LockstepEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\"N\n\x0cLockstepAxes\x12\x0e\n\x06\x61xis_1\x18\x01 \x01(\x05\x12\x0e\n\x06\x61xis_2\x18\x02 \x01(\x05\x12\x0e\n\x06\x61xis_3\x18\x03 \x01(\x05\x12\x0e\n\x06\x61xis_4\x18\x04 \x01(\x05\".\n\x1eLockstepGetAxisNumbersResponse\x12\x0c\n\x04\x61xes\x18\x01 \x03(\x05\"c\n\x12LockstepGetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x86\x01\n\x12LockstepSetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\x12\n\naxis_index\x18\x06 \x01(\x05\"k\n$OscilloscopeAddSettingChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\"l\n\x1fOscilloscopeAddIoChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07io_type\x18\x03 \x01(\x05\x12\x12\n\nio_channel\x18\x04 \x01(\x05\"k\n\x1cOscilloscopeStartStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\r\n\x05start\x18\x03 \x01(\x08\x12\x16\n\x0e\x63\x61pture_length\x18\x04 \x01(\x05\",\n\x18OscilloscopeReadResponse\x12\x10\n\x08\x64\x61ta_ids\x18\x01 \x03(\x05\"-\n\x1aOscilloscopeDataIdentifier\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\"\x7f\n\x1dOscilloscopeCaptureProperties\x12\x13\n\x0b\x64\x61ta_source\x18\x01 \x01(\x05\x12\x0f\n\x07setting\x18\x02 \x01(\t\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0f\n\x07io_type\x18\x04 \x01(\x05\x12\x12\n\nio_channel\x18\x05 \x01(\x05\";\n\x1aOscilloscopeDataGetRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\"T\n$OscilloscopeDataGetSampleTimeRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\"2\n\"OscilloscopeDataGetSamplesResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x01\"l\n\x16StreamSetupLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04\x61xes\x18\x05 \x03(\x05\"\xa3\x01\n\x1fStreamSetupLiveCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04\x61xes\x18\x05 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\x98\x01\n\x17StreamSetupStoreRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x07 \x03(\x05\"\xcf\x01\n StreamSetupStoreCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12:\n\x04\x61xes\x18\x07 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\xab\x01\n$StreamSetupStoreArbitraryAxesRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x12\n\naxes_count\x18\x07 \x01(\x05\"\x84\x01\n\x11StreamCallRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\"\xd1\x02\n\x0fPvtPointRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04type\x18\x05 \x01(\x0e\x32,.zaber.motion.protobufs.PvtPointRequest.Type\x12\x36\n\tpositions\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x37\n\nvelocities\x18\x07 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x31\n\x04time\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x85\x02\n\x11StreamLineRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12<\n\x04type\x18\x05 \x01(\x0e\x32..zaber.motion.protobufs.StreamLineRequest.Type\x12\x35\n\x08\x65ndpoint\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x07 \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xf5\x03\n\x10StreamArcRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12;\n\x04type\x18\x05 \x01(\x0e\x32-.zaber.motion.protobufs.StreamArcRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_x\x18\t \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_y\x18\n \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x0b \x03(\x05\x12\x35\n\x08\x65ndpoint\x18\x0c \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xdc\x02\n\x13StreamCircleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12>\n\x04type\x18\x05 \x01(\x0e\x32\x30.zaber.motion.protobufs.StreamCircleRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\t \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x8c\x01\n\x1dStreamWaitDigitalInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x9e\x01\n\x1cStreamWaitAnalogInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\x11\n\tcondition\x18\x06 \x01(\t\x12\r\n\x05value\x18\x07 \x01(\x01\"\x8c\x01\n\x1dStreamSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x8b\x01\n\x1cStreamSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x01\"\x80\x01\n StreamToggleDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\"y\n!StreamSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x08\"x\n StreamSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x01\"u\n\x11StreamWaitRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04time\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n\x1aStreamWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x1c\n\x14throw_error_on_fault\x18\x05 \x01(\x08\"Z\n\x12StreamEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"S\n\x15StreamGetAxesResponse\x12:\n\x04\x61xes\x18\x01 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"n\n\x18StreamGetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x81\x01\n\x18StreamSetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x05 \x01(\x08\x12\x11\n\tmax_speed\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\"\x7f\n)StreamGetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa4\x01\n)StreamSetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12#\n\x1bmax_tangential_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n*StreamGetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa6\x01\n*StreamSetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12$\n\x1cmax_centripetal_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"e\n\x1dStreamBufferGetContentRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"6\n\x1eStreamBufferGetContentResponse\x12\x14\n\x0c\x62uffer_lines\x18\x01 \x03(\t\"`\n\x18StreamBufferEraseRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"t\n\x1bStreamGenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0f\n\x07\x63ommand\x18\x05 \x01(\t\"w\n StreamGenericCommandBatchRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\r\n\x05\x62\x61tch\x18\x05 \x03(\t\"c\n\x14\x42inaryReplyOnlyEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\xbb\x01\n\x1aOpenBinaryInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x17\n\x0fuse_message_ids\x18\x06 \x01(\x08\"i\n\x1aUnknownBinaryResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\x82\x01\n\x14GenericBinaryRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x01\"F\n\rBinaryMessage\x12\x16\n\x0e\x64\x65vice_address\x18\x01 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x05\"R\n\x17\x42inaryMessageCollection\x12\x37\n\x08messages\x18\x02 \x03(\x0b\x32%.zaber.motion.protobufs.BinaryMessage\":\n\x12\x44\x65viceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\"\xd9\x02\n\x14\x42inaryDeviceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x15\n\ris_peripheral\x18\x06 \x01(\x08\x12\x15\n\rperipheral_id\x18\x07 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x08 \x01(\t\x12L\n\x0b\x64\x65vice_type\x18\t \x01(\x0e\x32\x37.zaber.motion.protobufs.BinaryDeviceIdentity.DeviceType\"1\n\nDeviceType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\x99\x01\n\x1d\x42inaryGenericWithUnitsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x01\x12\x11\n\tfrom_unit\x18\x05 \x01(\t\x12\x0f\n\x07to_unit\x18\x06 \x01(\t\x12\x0f\n\x07timeout\x18\x07 \x01(\x01\"^\n\x17\x42inaryDeviceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\xda\x01\n\x17\x42inaryDeviceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x46\n\x04type\x18\x04 \x01(\x0e\x32\x38.zaber.motion.protobufs.BinaryDeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"%\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\"^\n\x17\x42inaryDeviceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"K\n\x19\x42inaryDeviceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"-\n\x1a\x42inaryDeviceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"d\n\x1d\x42inaryDeviceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"s\n\x1d\x42inaryDeviceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"2\n\x1a\x43ustomInterfaceReadRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"D\n\x1b\x43ustomInterfaceWriteRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"3\n\x1b\x43ustomInterfaceOpenResponse\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"J\n\x1b\x43ustomInterfaceCloseRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"W\n\x12\x43\x61nSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\"=\n\x17\x43\x61nSetStateAxisResponse\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"p\n\x19\x43\x61nSetStateDeviceResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x44\n\x0b\x61xis_errors\x18\x02 \x03(\x0b\x32/.zaber.motion.protobufs.CanSetStateAxisResponse\"i\n\x0fSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65vice_only\x18\x05 \x01(\x08\"Z\n\x12ServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\"/\n\x10ServoTuningParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"g\n\x0cParamsetInfo\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x05\x12\x38\n\x06params\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"\x9e\x01\n\x15SetServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12?\n\rtuning_params\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"n\n\x0cLoadParamset\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x13\n\x0bto_paramset\x18\x04 \x01(\x05\x12\x15\n\rfrom_paramset\x18\x05 \x01(\x05\"\x8d\x01\n\x18SetServoTuningPIDRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\t\n\x01p\x18\x05 \x01(\x01\x12\t\n\x01i\x18\x06 \x01(\x01\x12\t\n\x01\x64\x18\x07 \x01(\x01\x12\n\n\x02\x66\x63\x18\x08 \x01(\x01\"W\n\tPidTuning\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\t\n\x01p\x18\x03 \x01(\x01\x12\t\n\x01i\x18\x04 \x01(\x01\x12\t\n\x01\x64\x18\x05 \x01(\x01\x12\n\n\x02\x66\x63\x18\x06 \x01(\x01\"\xc2\x01\n\x0fSetSimpleTuning\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\x15\n\rcarriage_mass\x18\x05 \x01(\x01\x12\x11\n\tload_mass\x18\x06 \x01(\x01\x12?\n\rtuning_params\x18\x07 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"d\n\x1bSimpleTuningParamDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tmin_label\x18\x02 \x01(\t\x12\x11\n\tmax_label\x18\x03 \x01(\t\x12\x11\n\tdata_type\x18\x04 \x01(\t\"m\n&GetSimpleTuningParamDefinitionResponse\x12\x43\n\x06params\x18\x01 \x03(\x0b\x32\x33.zaber.motion.protobufs.SimpleTuningParamDefinition\"\x95\x01\n\x17TranslatorCreateRequest\x12@\n\ndefinition\x18\x01 \x01(\x0b\x32,.zaber.motion.protobufs.TranslatorDefinition\x12\x38\n\x06\x63onfig\x18\x02 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"1\n\x18TranslatorCreateResponse\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"O\n\x18TranslatorAxisDefinition\x12\x15\n\rperipheral_id\x18\x01 \x01(\x05\x12\x1c\n\x14microstep_resolution\x18\x02 \x01(\x05\"\xa1\x01\n\x14TranslatorDefinition\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12>\n\x04\x61xes\x18\x02 \x03(\x0b\x32\x30.zaber.motion.protobufs.TranslatorAxisDefinition\x12\x36\n\tmax_speed\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\xac\x01\n\x10TranslatorConfig\x12\x44\n\raxis_mappings\x18\x01 \x03(\x0b\x32-.zaber.motion.protobufs.TranslatorAxisMapping\x12R\n\x14\x61xis_transformations\x18\x02 \x03(\x0b\x32\x34.zaber.motion.protobufs.TranslatorAxisTransformation\"@\n\x15TranslatorAxisMapping\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x12\n\naxis_index\x18\x02 \x01(\x05\"~\n\x1cTranslatorAxisTransformation\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x0f\n\x07scaling\x18\x02 \x01(\x01\x12\x38\n\x0btranslation\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"B\n\x1aTranslatorTranslateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\r\n\x05\x62lock\x18\x02 \x01(\t\"I\n\x10TranslateMessage\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x12\n\nfrom_block\x18\x02 \x01(\x05\x12\x10\n\x08to_block\x18\x03 \x01(\x05\"k\n\x1bTranslatorTranslateResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\x12:\n\x08warnings\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.TranslateMessage\"@\n\x18GCodeSyntaxExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"C\n\x1bGCodeExecutionExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"L\n\x1aTranslatorFlushLiveRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"+\n\x17TranslatorFlushResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\"\x90\x01\n\x1bTranslatorCreateLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"\x91\x01\n!TranslatorCreateFromDeviceRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x03 \x03(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"/\n\x16TranslatorEmptyRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"^\n TranslatorSetTraverseRateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x15\n\rtraverse_rate\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"g\n TranslatorSetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x10\n\x08position\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"U\n TranslatorGetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x0c\n\x04unit\x18\x03 \x01(\t\"n\n\x1eTranslatorGetAxisOffsetRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x19\n\x11\x63oordinate_system\x18\x02 \x01(\t\x12\x0c\n\x04\x61xis\x18\x03 \x01(\t\x12\x0c\n\x04unit\x18\x04 \x01(\t\"R\n$TranslatorSetFeedRateOverrideRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x13\n\x0b\x63oefficient\x18\x02 \x01(\x01\"y\n\x17\x44\x65viceSetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\x12\x0e\n\x06\x65ncode\x18\x06 \x01(\x08\"j\n\x17\x44\x65viceGetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\x0e\n\x06\x64\x65\x63ode\x18\x05 \x01(\x08\"o\n\x1d\x44\x65viceSetStorageNumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\"m\n\x1b\x44\x65viceSetStorageBoolRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x08\"W\n\x14\x44\x65viceStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\"b\n\x1c\x44\x65viceStorageListKeysRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0e\n\x06prefix\x18\x04 \x01(\t\"\xa1\x01\n\x1f\x44\x65viceSetUnitConversionsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12=\n\x0b\x63onversions\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ConversionFactor\"@\n\x10\x43onversionFactor\x12\x0f\n\x07setting\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"^\n\x17ObjectiveChangerRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\"?\n\x1eObjectiveChangerCreateResponse\x12\x0e\n\x06turret\x18\x02 \x01(\x05\x12\r\n\x05\x66ocus\x18\x03 \x01(\x05\"\xb2\x01\n\x1dObjectiveChangerChangeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\x12\x11\n\tobjective\x18\x04 \x01(\x05\x12\x39\n\x0c\x66ocus_offset\x18\x05 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"3\n\"ObjectiveChangerGetCurrentResponse\x12\r\n\x05value\x18\x01 \x01(\x05\"]\n\tProcessOn\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\n\n\x02on\x18\x04 \x01(\x08\x12\x10\n\x08\x64uration\x18\x05 \x01(\x01\"7\n\x17ProcessControllerSource\x12\x0e\n\x06sensor\x18\x01 \x01(\x05\x12\x0c\n\x04port\x18\x02 \x01(\x05\"\x91\x01\n\x1aSetProcessControllerSource\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12?\n\x06source\x18\x04 \x01(\x0b\x32/.zaber.motion.protobufs.ProcessControllerSource*-\n\x0bMessageType\x12\t\n\x05REPLY\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\t\n\x05\x41LERT\x10\x02*\xc0\t\n\x06\x45rrors\x12\x13\n\x0fREQUEST_TIMEOUT\x10\x00\x12\x15\n\x11\x43ONNECTION_CLOSED\x10\x01\x12\x14\n\x10INVALID_ARGUMENT\x10\x02\x12\x16\n\x12OUT_OF_REQUEST_IDS\x10\x03\x12\x12\n\x0eINVALID_PACKET\x10\x04\x12\x15\n\x11\x43ONNECTION_FAILED\x10\x05\x12\x13\n\x0fUNKNOWN_REQUEST\x10\x06\x12\x12\n\x0e\x43OMMAND_FAILED\x10\x07\x12\x14\n\x10\x44\x45VICE_DB_FAILED\x10\x08\x12\x10\n\x0cINVALID_DATA\x10\t\x12\x19\n\x15\x44\x45VICE_NOT_IDENTIFIED\x10\n\x12\x15\n\x11\x43ONVERSION_FAILED\x10\x0b\x12\x1b\n\x17\x44\x45VICE_ADDRESS_CONFLICT\x10\x0c\x12\x13\n\x0fNO_DEVICE_FOUND\x10\r\x12\x18\n\x14MOVEMENT_INTERRUPTED\x10\x0e\x12\x13\n\x0fMOVEMENT_FAILED\x10\x0f\x12\r\n\tIO_FAILED\x10\x10\x12\x14\n\x10INVALID_RESPONSE\x10\x11\x12\x11\n\rNOT_SUPPORTED\x10\x12\x12\x11\n\rDEVICE_FAILED\x10\x13\x12\r\n\tOS_FAILED\x10\x14\x12\x12\n\x0eINTERNAL_ERROR\x10\x16\x12\x19\n\x15\x42INARY_COMMAND_FAILED\x10\x18\x12\x15\n\x11\x43OMMAND_PREEMPTED\x10\x19\x12\x18\n\x14LOCKSTEP_NOT_ENABLED\x10\x1a\x12\x14\n\x10LOCKSTEP_ENABLED\x10\x1b\x12\x1b\n\x17IO_CHANNEL_OUT_OF_RANGE\x10\x1c\x12\x15\n\x11SETTING_NOT_FOUND\x10\x1d\x12\x0f\n\x0bSTREAM_MODE\x10\x1e\x12\x14\n\x10STREAM_EXECUTION\x10\x1f\x12\x1a\n\x16STREAM_MOVEMENT_FAILED\x10 \x12\x17\n\x13STREAM_SETUP_FAILED\x10!\x12\x0f\n\x0b\x44\x45VICE_BUSY\x10\"\x12\x1f\n\x1bSTREAM_MOVEMENT_INTERRUPTED\x10#\x12\x16\n\x12INVALID_PARK_STATE\x10$\x12\x14\n\x10SERIAL_PORT_BUSY\x10%\x12\x1a\n\x16TRANSPORT_ALREADY_USED\x10&\x12\x1f\n\x1bSET_PERIPHERAL_STATE_FAILED\x10\'\x12\x1b\n\x17SET_DEVICE_STATE_FAILED\x10(\x12\x11\n\rG_CODE_SYNTAX\x10)\x12\x14\n\x10G_CODE_EXECUTION\x10*\x12\x15\n\x11INVALID_OPERATION\x10+\x12\x14\n\x10\x43OMMAND_TOO_LONG\x10,\x12\x14\n\x10NO_VALUE_FOR_KEY\x10-\x12\x1b\n\x17\x44\x45VICE_DETECTION_FAILED\x10.\x12\x0b\n\x07TIMEOUT\x10/\x12\x0c\n\x08PVT_MODE\x10\x30\x12\x11\n\rPVT_EXECUTION\x10\x31\x12\x14\n\x10PVT_SETUP_FAILED\x10\x32\x12\x17\n\x13PVT_MOVEMENT_FAILED\x10\x33\x12\x1c\n\x18PVT_MOVEMENT_INTERRUPTED\x10\x34\x12\x15\n\x11PVT_DISCONTINUITY\x10\x35\x12\x18\n\x14STREAM_DISCONTINUITY\x10\x36*Q\n\rInterfaceType\x12\x0f\n\x0bSERIAL_PORT\x10\x00\x12\x07\n\x03TCP\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\x07\n\x03IOT\x10\x03\x12\x11\n\rNETWORK_SHARE\x10\x04\x42$Z\"./protobufs;zaber_motion_protobufsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protobufs.main_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\"./protobufs;zaber_motion_protobufs'
-  _MESSAGETYPE._serialized_start=22861
-  _MESSAGETYPE._serialized_end=22906
-  _ERRORS._serialized_start=22909
-  _ERRORS._serialized_end=24125
-  _INTERFACETYPE._serialized_start=24127
-  _INTERFACETYPE._serialized_end=24208
+  _MESSAGETYPE._serialized_start=22890
+  _MESSAGETYPE._serialized_end=22935
+  _ERRORS._serialized_start=22938
+  _ERRORS._serialized_end=24154
+  _INTERFACETYPE._serialized_start=24156
+  _INTERFACETYPE._serialized_end=24237
   _REQUEST._serialized_start=48
   _REQUEST._serialized_end=74
   _RESPONSE._serialized_start=77
   _RESPONSE._serialized_end=262
   _RESPONSE_RESPONSETYPE._serialized_start=229
   _RESPONSE_RESPONSETYPE._serialized_end=262
   _EVENT._serialized_start=264
   _EVENT._serialized_end=286
   _EMPTYREQUEST._serialized_start=288
   _EMPTYREQUEST._serialized_end=302
-  _BOOLRESPONSE._serialized_start=304
-  _BOOLRESPONSE._serialized_end=333
-  _DOUBLERESPONSE._serialized_start=335
-  _DOUBLERESPONSE._serialized_end=366
-  _DOUBLEARRAYRESPONSE._serialized_start=368
-  _DOUBLEARRAYRESPONSE._serialized_end=405
-  _INTRESPONSE._serialized_start=407
-  _INTRESPONSE._serialized_end=435
-  _STRINGRESPONSE._serialized_start=437
-  _STRINGRESPONSE._serialized_end=468
-  _STRINGARRAYRESPONSE._serialized_start=470
-  _STRINGARRAYRESPONSE._serialized_end=507
-  _AXISIDENTITY._serialized_start=510
-  _AXISIDENTITY._serialized_end=731
-  _AXISIDENTITY_AXISTYPE._serialized_start=684
-  _AXISIDENTITY_AXISTYPE._serialized_end=731
-  _DEVICEIDENTITY._serialized_start=734
-  _DEVICEIDENTITY._serialized_end=937
-  _FIRMWAREVERSION._serialized_start=939
-  _FIRMWAREVERSION._serialized_end=1001
-  _DEVICEIOINFO._serialized_start=1004
-  _DEVICEIOINFO._serialized_end=1142
-  _MEASUREMENT._serialized_start=1144
-  _MEASUREMENT._serialized_end=1203
-  _STREAMAXISDEFINITION._serialized_start=1205
-  _STREAMAXISDEFINITION._serialized_end=1267
-  _INVALIDPACKETEXCEPTIONDATA._serialized_start=1269
-  _INVALIDPACKETEXCEPTIONDATA._serialized_end=1329
-  _DEVICEADDRESSCONFLICTEXCEPTIONDATA._serialized_start=1331
-  _DEVICEADDRESSCONFLICTEXCEPTIONDATA._serialized_end=1393
-  _MOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_start=1395
-  _MOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_end=1493
-  _STREAMMOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_start=1495
-  _STREAMMOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_end=1569
-  _PVTMOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_start=1571
-  _PVTMOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_end=1642
-  _MOVEMENTFAILEDEXCEPTIONDATA._serialized_start=1644
-  _MOVEMENTFAILEDEXCEPTIONDATA._serialized_end=1737
-  _STREAMMOVEMENTFAILEDEXCEPTIONDATA._serialized_start=1739
-  _STREAMMOVEMENTFAILEDEXCEPTIONDATA._serialized_end=1808
-  _PVTMOVEMENTFAILEDEXCEPTIONDATA._serialized_start=1810
-  _PVTMOVEMENTFAILEDEXCEPTIONDATA._serialized_end=1876
-  _STREAMEXECUTIONEXCEPTIONDATA._serialized_start=1878
-  _STREAMEXECUTIONEXCEPTIONDATA._serialized_end=1944
-  _PVTEXECUTIONEXCEPTIONDATA._serialized_start=1947
-  _PVTEXECUTIONEXCEPTIONDATA._serialized_end=2075
-  _INVALIDPVTPOINT._serialized_start=2077
-  _INVALIDPVTPOINT._serialized_end=2124
-  _INVALIDRESPONSEEXCEPTIONDATA._serialized_start=2126
-  _INVALIDRESPONSEEXCEPTIONDATA._serialized_end=2174
-  _COMMANDFAILEDEXCEPTIONDATA._serialized_start=2177
-  _COMMANDFAILEDEXCEPTIONDATA._serialized_end=2360
-  _BINARYCOMMANDFAILEDEXCEPTIONDATA._serialized_start=2362
-  _BINARYCOMMANDFAILEDEXCEPTIONDATA._serialized_end=2419
-  _SETPERIPHERALSTATEEXCEPTIONDATA._serialized_start=2422
-  _SETPERIPHERALSTATEEXCEPTIONDATA._serialized_end=2559
-  _SETDEVICESTATEEXCEPTIONDATA._serialized_start=2562
-  _SETDEVICESTATEEXCEPTIONDATA._serialized_end=2815
-  _COMMANDTOOLONGEXCEPTIONDATA._serialized_start=2817
-  _COMMANDTOOLONGEXCEPTIONDATA._serialized_end=2920
-  _TESTREQUEST._serialized_start=2922
-  _TESTREQUEST._serialized_end=3008
-  _TESTRESPONSE._serialized_start=3010
-  _TESTRESPONSE._serialized_end=3043
-  _TESTRESPONSELONG._serialized_start=3045
-  _TESTRESPONSELONG._serialized_end=3082
-  _TESTEVENT._serialized_start=3084
-  _TESTEVENT._serialized_end=3109
-  _TOOLSLISTSERIALPORTSRESPONSE._serialized_start=3111
-  _TOOLSLISTSERIALPORTSRESPONSE._serialized_end=3156
-  _SETINTERNALMODEREQUEST._serialized_start=3158
-  _SETINTERNALMODEREQUEST._serialized_end=3196
-  _SETDEVICEDBSOURCEREQUEST._serialized_start=3198
-  _SETDEVICEDBSOURCEREQUEST._serialized_end=3271
-  _TOGGLEDEVICEDBSTOREREQUEST._serialized_start=3273
-  _TOGGLEDEVICEDBSTOREREQUEST._serialized_end=3344
-  _DEVICEDBFAILEDEXCEPTIONDATA._serialized_start=3346
-  _DEVICEDBFAILEDEXCEPTIONDATA._serialized_end=3389
-  _OPENINTERFACEREQUEST._serialized_start=3392
-  _OPENINTERFACEREQUEST._serialized_end=3687
-  _OPENINTERFACERESPONSE._serialized_start=3689
-  _OPENINTERFACERESPONSE._serialized_end=3734
-  _INTERFACEEMPTYREQUEST._serialized_start=3736
-  _INTERFACEEMPTYREQUEST._serialized_end=3781
-  _SETINTERFACETIMEOUTREQUEST._serialized_start=3783
-  _SETINTERFACETIMEOUTREQUEST._serialized_end=3850
-  _SETINTERFACECHECKSUMENABLEDREQUEST._serialized_start=3852
-  _SETINTERFACECHECKSUMENABLEDREQUEST._serialized_end=3930
-  _AXISEMPTYREQUEST._serialized_start=3932
-  _AXISEMPTYREQUEST._serialized_end=4002
-  _GENERICCOMMANDREQUEST._serialized_start=4005
-  _GENERICCOMMANDREQUEST._serialized_end=4136
-  _GENERICCOMMANDRESPONSE._serialized_start=4139
-  _GENERICCOMMANDRESPONSE._serialized_end=4339
-  _GENERICCOMMANDRESPONSECOLLECTION._serialized_start=4341
-  _GENERICCOMMANDRESPONSECOLLECTION._serialized_end=4442
-  _UNKNOWNRESPONSEEVENT._serialized_start=4445
-  _UNKNOWNRESPONSEEVENT._serialized_end=4665
-  _ALERTEVENT._serialized_start=4668
-  _ALERTEVENT._serialized_end=4799
-  _DISCONNECTEDEVENT._serialized_start=4801
-  _DISCONNECTEDEVENT._serialized_end=4917
-  _DEVICEIDENTIFYREQUEST._serialized_start=4919
-  _DEVICEIDENTIFYREQUEST._serialized_end=5045
-  _DEVICERENUMBERREQUEST._serialized_start=5047
-  _DEVICERENUMBERREQUEST._serialized_end=5115
-  _DEVICEDETECTREQUEST._serialized_start=5118
-  _DEVICEDETECTREQUEST._serialized_end=5304
-  _DEVICEDETECTREQUEST_DEVICETYPE._serialized_start=5259
-  _DEVICEDETECTREQUEST_DEVICETYPE._serialized_end=5304
-  _DEVICEDETECTRESPONSE._serialized_start=5306
-  _DEVICEDETECTRESPONSE._serialized_end=5345
-  _DEVICEHOMEREQUEST._serialized_start=5347
-  _DEVICEHOMEREQUEST._serialized_end=5443
-  _DEVICEWAITUNTILIDLEREQUEST._serialized_start=5445
-  _DEVICEWAITUNTILIDLEREQUEST._serialized_end=5555
-  _DEVICEMOVEREQUEST._serialized_start=5558
-  _DEVICEMOVEREQUEST._serialized_end=5894
-  _DEVICEMOVEREQUEST_MOVETYPE._serialized_start=5839
-  _DEVICEMOVEREQUEST_MOVETYPE._serialized_end=5894
-  _DEVICESTOPREQUEST._serialized_start=5896
-  _DEVICESTOPREQUEST._serialized_end=5992
-  _DEVICEONALLREQUEST._serialized_start=5994
-  _DEVICEONALLREQUEST._serialized_end=6061
-  _DEVICEONALLRESPONSE._serialized_start=6063
-  _DEVICEONALLRESPONSE._serialized_end=6110
-  _DEVICEGETWARNINGSREQUEST._serialized_start=6112
-  _DEVICEGETWARNINGSREQUEST._serialized_end=6205
-  _DEVICEGETWARNINGSRESPONSE._serialized_start=6207
-  _DEVICEGETWARNINGSRESPONSE._serialized_end=6249
-  _WAITTOCLEARWARNINGSREQUEST._serialized_start=6251
-  _WAITTOCLEARWARNINGSREQUEST._serialized_end=6371
-  _DEVICEGETALLDIGITALIOREQUEST._serialized_start=6373
-  _DEVICEGETALLDIGITALIOREQUEST._serialized_end=6463
-  _DEVICEGETALLDIGITALIORESPONSE._serialized_start=6465
-  _DEVICEGETALLDIGITALIORESPONSE._serialized_end=6512
-  _DEVICEGETALLANALOGIOREQUEST._serialized_start=6514
-  _DEVICEGETALLANALOGIOREQUEST._serialized_end=6603
-  _DEVICEGETALLANALOGIORESPONSE._serialized_start=6605
-  _DEVICEGETALLANALOGIORESPONSE._serialized_end=6651
-  _DEVICEGETDIGITALIOREQUEST._serialized_start=6653
-  _DEVICEGETDIGITALIOREQUEST._serialized_end=6764
-  _DEVICEGETANALOGIOREQUEST._serialized_start=6766
-  _DEVICEGETANALOGIOREQUEST._serialized_end=6876
-  _DEVICESETALLDIGITALOUTPUTSREQUEST._serialized_start=6878
-  _DEVICESETALLDIGITALOUTPUTSREQUEST._serialized_end=6967
-  _DEVICESETALLANALOGOUTPUTSREQUEST._serialized_start=6969
-  _DEVICESETALLANALOGOUTPUTSREQUEST._serialized_end=7057
-  _DEVICESETDIGITALOUTPUTREQUEST._serialized_start=7059
-  _DEVICESETDIGITALOUTPUTREQUEST._serialized_end=7167
-  _DEVICESETANALOGOUTPUTREQUEST._serialized_start=7169
-  _DEVICESETANALOGOUTPUTREQUEST._serialized_end=7276
-  _SETLOGOUTPUTREQUEST._serialized_start=7278
-  _SETLOGOUTPUTREQUEST._serialized_end=7332
-  _DEVICEGETSETTINGREQUEST._serialized_start=7334
-  _DEVICEGETSETTINGREQUEST._serialized_end=7442
-  _DEVICECONVERTSETTINGREQUEST._serialized_start=7445
-  _DEVICECONVERTSETTINGREQUEST._serialized_end=7593
-  _DEVICESETSETTINGREQUEST._serialized_start=7595
-  _DEVICESETSETTINGREQUEST._serialized_end=7718
-  _DEVICESETSETTINGSTRREQUEST._serialized_start=7720
-  _DEVICESETSETTINGSTRREQUEST._serialized_end=7832
-  _PREPARECOMMANDREQUEST._serialized_start=7835
-  _PREPARECOMMANDREQUEST._serialized_end=7993
-  _WAITTORESPONDREQUEST._serialized_start=7995
-  _WAITTORESPONDREQUEST._serialized_end=8072
-  _LOCKSTEPENABLEREQUEST._serialized_start=8074
-  _LOCKSTEPENABLEREQUEST._serialized_end=8176
-  _LOCKSTEPDISABLEREQUEST._serialized_start=8178
-  _LOCKSTEPDISABLEREQUEST._serialized_end=8292
-  _LOCKSTEPSTOPREQUEST._serialized_start=8294
-  _LOCKSTEPSTOPREQUEST._serialized_end=8405
-  _LOCKSTEPHOMEREQUEST._serialized_start=8407
-  _LOCKSTEPHOMEREQUEST._serialized_end=8518
-  _LOCKSTEPMOVEREQUEST._serialized_start=8521
-  _LOCKSTEPMOVEREQUEST._serialized_end=8874
-  _LOCKSTEPMOVEREQUEST_MOVETYPE._serialized_start=5839
-  _LOCKSTEPMOVEREQUEST_MOVETYPE._serialized_end=5894
-  _LOCKSTEPWAITUNTILIDLEREQUEST._serialized_start=8876
-  _LOCKSTEPWAITUNTILIDLEREQUEST._serialized_end=9001
-  _LOCKSTEPEMPTYREQUEST._serialized_start=9003
-  _LOCKSTEPEMPTYREQUEST._serialized_end=9090
-  _LOCKSTEPAXES._serialized_start=9092
-  _LOCKSTEPAXES._serialized_end=9170
-  _LOCKSTEPGETAXISNUMBERSRESPONSE._serialized_start=9172
-  _LOCKSTEPGETAXISNUMBERSRESPONSE._serialized_end=9218
-  _LOCKSTEPGETREQUEST._serialized_start=9220
-  _LOCKSTEPGETREQUEST._serialized_end=9319
-  _LOCKSTEPSETREQUEST._serialized_start=9322
-  _LOCKSTEPSETREQUEST._serialized_end=9456
-  _OSCILLOSCOPEADDSETTINGCHANNELREQUEST._serialized_start=9458
-  _OSCILLOSCOPEADDSETTINGCHANNELREQUEST._serialized_end=9565
-  _OSCILLOSCOPEADDIOCHANNELREQUEST._serialized_start=9567
-  _OSCILLOSCOPEADDIOCHANNELREQUEST._serialized_end=9675
-  _OSCILLOSCOPESTARTSTOPREQUEST._serialized_start=9677
-  _OSCILLOSCOPESTARTSTOPREQUEST._serialized_end=9784
-  _OSCILLOSCOPEREADRESPONSE._serialized_start=9786
-  _OSCILLOSCOPEREADRESPONSE._serialized_end=9830
-  _OSCILLOSCOPEDATAIDENTIFIER._serialized_start=9832
-  _OSCILLOSCOPEDATAIDENTIFIER._serialized_end=9877
-  _OSCILLOSCOPECAPTUREPROPERTIES._serialized_start=9879
-  _OSCILLOSCOPECAPTUREPROPERTIES._serialized_end=10006
-  _OSCILLOSCOPEDATAGETREQUEST._serialized_start=10008
-  _OSCILLOSCOPEDATAGETREQUEST._serialized_end=10067
-  _OSCILLOSCOPEDATAGETSAMPLETIMEREQUEST._serialized_start=10069
-  _OSCILLOSCOPEDATAGETSAMPLETIMEREQUEST._serialized_end=10153
-  _OSCILLOSCOPEDATAGETSAMPLESRESPONSE._serialized_start=10155
-  _OSCILLOSCOPEDATAGETSAMPLESRESPONSE._serialized_end=10205
-  _STREAMSETUPLIVEREQUEST._serialized_start=10207
-  _STREAMSETUPLIVEREQUEST._serialized_end=10315
-  _STREAMSETUPLIVECOMPOSITEREQUEST._serialized_start=10318
-  _STREAMSETUPLIVECOMPOSITEREQUEST._serialized_end=10481
-  _STREAMSETUPSTOREREQUEST._serialized_start=10484
-  _STREAMSETUPSTOREREQUEST._serialized_end=10636
-  _STREAMSETUPSTORECOMPOSITEREQUEST._serialized_start=10639
-  _STREAMSETUPSTORECOMPOSITEREQUEST._serialized_end=10846
-  _STREAMSETUPSTOREARBITRARYAXESREQUEST._serialized_start=10849
-  _STREAMSETUPSTOREARBITRARYAXESREQUEST._serialized_end=11020
-  _STREAMCALLREQUEST._serialized_start=11023
-  _STREAMCALLREQUEST._serialized_end=11155
-  _PVTPOINTREQUEST._serialized_start=11158
-  _PVTPOINTREQUEST._serialized_end=11495
-  _PVTPOINTREQUEST_TYPE._serialized_start=11471
-  _PVTPOINTREQUEST_TYPE._serialized_end=11495
-  _STREAMLINEREQUEST._serialized_start=11498
-  _STREAMLINEREQUEST._serialized_end=11759
-  _STREAMLINEREQUEST_TYPE._serialized_start=11471
-  _STREAMLINEREQUEST_TYPE._serialized_end=11495
-  _STREAMARCREQUEST._serialized_start=11762
-  _STREAMARCREQUEST._serialized_end=12263
-  _STREAMARCREQUEST_TYPE._serialized_start=11471
-  _STREAMARCREQUEST_TYPE._serialized_end=11495
-  _STREAMCIRCLEREQUEST._serialized_start=12266
-  _STREAMCIRCLEREQUEST._serialized_end=12614
-  _STREAMCIRCLEREQUEST_TYPE._serialized_start=11471
-  _STREAMCIRCLEREQUEST_TYPE._serialized_end=11495
-  _STREAMWAITDIGITALINPUTREQUEST._serialized_start=12617
-  _STREAMWAITDIGITALINPUTREQUEST._serialized_end=12757
-  _STREAMWAITANALOGINPUTREQUEST._serialized_start=12760
-  _STREAMWAITANALOGINPUTREQUEST._serialized_end=12918
-  _STREAMSETDIGITALOUTPUTREQUEST._serialized_start=12921
-  _STREAMSETDIGITALOUTPUTREQUEST._serialized_end=13061
-  _STREAMSETANALOGOUTPUTREQUEST._serialized_start=13064
-  _STREAMSETANALOGOUTPUTREQUEST._serialized_end=13203
-  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_start=13206
-  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_end=13334
-  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_start=13336
-  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_end=13457
-  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_start=13459
-  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_end=13579
-  _STREAMWAITREQUEST._serialized_start=13581
-  _STREAMWAITREQUEST._serialized_end=13698
-  _STREAMWAITUNTILIDLEREQUEST._serialized_start=13701
-  _STREAMWAITUNTILIDLEREQUEST._serialized_end=13829
-  _STREAMEMPTYREQUEST._serialized_start=13831
-  _STREAMEMPTYREQUEST._serialized_end=13921
-  _STREAMGETAXESRESPONSE._serialized_start=13923
-  _STREAMGETAXESRESPONSE._serialized_end=14006
-  _STREAMGETMAXSPEEDREQUEST._serialized_start=14008
-  _STREAMGETMAXSPEEDREQUEST._serialized_end=14118
-  _STREAMSETMAXSPEEDREQUEST._serialized_start=14121
-  _STREAMSETMAXSPEEDREQUEST._serialized_end=14250
-  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=14252
-  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=14379
-  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=14382
-  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=14546
-  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=14549
-  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=14677
-  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=14680
-  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=14846
-  _STREAMBUFFERGETCONTENTREQUEST._serialized_start=14848
-  _STREAMBUFFERGETCONTENTREQUEST._serialized_end=14949
-  _STREAMBUFFERGETCONTENTRESPONSE._serialized_start=14951
-  _STREAMBUFFERGETCONTENTRESPONSE._serialized_end=15005
-  _STREAMBUFFERERASEREQUEST._serialized_start=15007
-  _STREAMBUFFERERASEREQUEST._serialized_end=15103
-  _STREAMGENERICCOMMANDREQUEST._serialized_start=15105
-  _STREAMGENERICCOMMANDREQUEST._serialized_end=15221
-  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_start=15223
-  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_end=15342
-  _BINARYREPLYONLYEVENT._serialized_start=15344
-  _BINARYREPLYONLYEVENT._serialized_end=15443
-  _OPENBINARYINTERFACEREQUEST._serialized_start=15446
-  _OPENBINARYINTERFACEREQUEST._serialized_end=15633
-  _UNKNOWNBINARYRESPONSEEVENT._serialized_start=15635
-  _UNKNOWNBINARYRESPONSEEVENT._serialized_end=15740
-  _GENERICBINARYREQUEST._serialized_start=15743
-  _GENERICBINARYREQUEST._serialized_end=15873
-  _BINARYMESSAGE._serialized_start=15875
-  _BINARYMESSAGE._serialized_end=15945
-  _BINARYMESSAGECOLLECTION._serialized_start=15947
-  _BINARYMESSAGECOLLECTION._serialized_end=16029
-  _DEVICEEMPTYREQUEST._serialized_start=16031
-  _DEVICEEMPTYREQUEST._serialized_end=16089
-  _BINARYDEVICEIDENTITY._serialized_start=16092
-  _BINARYDEVICEIDENTITY._serialized_end=16437
-  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_start=16388
-  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_end=16437
-  _BINARYGENERICWITHUNITSREQUEST._serialized_start=16440
-  _BINARYGENERICWITHUNITSREQUEST._serialized_end=16593
-  _BINARYDEVICEHOMEREQUEST._serialized_start=16595
-  _BINARYDEVICEHOMEREQUEST._serialized_end=16689
-  _BINARYDEVICEMOVEREQUEST._serialized_start=16692
-  _BINARYDEVICEMOVEREQUEST._serialized_end=16910
-  _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_start=5839
-  _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_end=5876
-  _BINARYDEVICESTOPREQUEST._serialized_start=16912
-  _BINARYDEVICESTOPREQUEST._serialized_end=17006
-  _BINARYDEVICEDETECTREQUEST._serialized_start=17008
-  _BINARYDEVICEDETECTREQUEST._serialized_end=17083
-  _BINARYDEVICEDETECTRESPONSE._serialized_start=17085
-  _BINARYDEVICEDETECTRESPONSE._serialized_end=17130
-  _BINARYDEVICEGETSETTINGREQUEST._serialized_start=17132
-  _BINARYDEVICEGETSETTINGREQUEST._serialized_end=17232
-  _BINARYDEVICESETSETTINGREQUEST._serialized_start=17234
-  _BINARYDEVICESETSETTINGREQUEST._serialized_end=17349
-  _CUSTOMINTERFACEREADREQUEST._serialized_start=17351
-  _CUSTOMINTERFACEREADREQUEST._serialized_end=17401
-  _CUSTOMINTERFACEWRITEREQUEST._serialized_start=17403
-  _CUSTOMINTERFACEWRITEREQUEST._serialized_end=17471
-  _CUSTOMINTERFACEOPENRESPONSE._serialized_start=17473
-  _CUSTOMINTERFACEOPENRESPONSE._serialized_end=17524
-  _CUSTOMINTERFACECLOSEREQUEST._serialized_start=17526
-  _CUSTOMINTERFACECLOSEREQUEST._serialized_end=17600
-  _CANSETSTATEREQUEST._serialized_start=17602
-  _CANSETSTATEREQUEST._serialized_end=17689
-  _CANSETSTATEAXISRESPONSE._serialized_start=17691
-  _CANSETSTATEAXISRESPONSE._serialized_end=17752
-  _CANSETSTATEDEVICERESPONSE._serialized_start=17754
-  _CANSETSTATEDEVICERESPONSE._serialized_end=17866
-  _SETSTATEREQUEST._serialized_start=17868
-  _SETSTATEREQUEST._serialized_end=17973
-  _SERVOTUNINGREQUEST._serialized_start=17975
-  _SERVOTUNINGREQUEST._serialized_end=18065
-  _SERVOTUNINGPARAM._serialized_start=18067
-  _SERVOTUNINGPARAM._serialized_end=18114
-  _PARAMSETINFO._serialized_start=18116
-  _PARAMSETINFO._serialized_end=18219
-  _SETSERVOTUNINGREQUEST._serialized_start=18222
-  _SETSERVOTUNINGREQUEST._serialized_end=18380
-  _LOADPARAMSET._serialized_start=18382
-  _LOADPARAMSET._serialized_end=18492
-  _SETSERVOTUNINGPIDREQUEST._serialized_start=18495
-  _SETSERVOTUNINGPIDREQUEST._serialized_end=18636
-  _PIDTUNING._serialized_start=18638
-  _PIDTUNING._serialized_end=18725
-  _SETSIMPLETUNING._serialized_start=18728
-  _SETSIMPLETUNING._serialized_end=18922
-  _SIMPLETUNINGPARAMDEFINITION._serialized_start=18924
-  _SIMPLETUNINGPARAMDEFINITION._serialized_end=19024
-  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_start=19026
-  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_end=19135
-  _TRANSLATORCREATEREQUEST._serialized_start=19138
-  _TRANSLATORCREATEREQUEST._serialized_end=19287
-  _TRANSLATORCREATERESPONSE._serialized_start=19289
-  _TRANSLATORCREATERESPONSE._serialized_end=19338
-  _TRANSLATORAXISDEFINITION._serialized_start=19340
-  _TRANSLATORAXISDEFINITION._serialized_end=19419
-  _TRANSLATORDEFINITION._serialized_start=19422
-  _TRANSLATORDEFINITION._serialized_end=19583
-  _TRANSLATORCONFIG._serialized_start=19586
-  _TRANSLATORCONFIG._serialized_end=19758
-  _TRANSLATORAXISMAPPING._serialized_start=19760
-  _TRANSLATORAXISMAPPING._serialized_end=19824
-  _TRANSLATORAXISTRANSFORMATION._serialized_start=19826
-  _TRANSLATORAXISTRANSFORMATION._serialized_end=19952
-  _TRANSLATORTRANSLATEREQUEST._serialized_start=19954
-  _TRANSLATORTRANSLATEREQUEST._serialized_end=20020
-  _TRANSLATEMESSAGE._serialized_start=20022
-  _TRANSLATEMESSAGE._serialized_end=20095
-  _TRANSLATORTRANSLATERESPONSE._serialized_start=20097
-  _TRANSLATORTRANSLATERESPONSE._serialized_end=20204
-  _GCODESYNTAXEXCEPTIONDATA._serialized_start=20206
-  _GCODESYNTAXEXCEPTIONDATA._serialized_end=20270
-  _GCODEEXECUTIONEXCEPTIONDATA._serialized_start=20272
-  _GCODEEXECUTIONEXCEPTIONDATA._serialized_end=20339
-  _TRANSLATORFLUSHLIVEREQUEST._serialized_start=20341
-  _TRANSLATORFLUSHLIVEREQUEST._serialized_end=20417
-  _TRANSLATORFLUSHRESPONSE._serialized_start=20419
-  _TRANSLATORFLUSHRESPONSE._serialized_end=20462
-  _TRANSLATORCREATELIVEREQUEST._serialized_start=20465
-  _TRANSLATORCREATELIVEREQUEST._serialized_end=20609
-  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_start=20612
-  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_end=20757
-  _TRANSLATOREMPTYREQUEST._serialized_start=20759
-  _TRANSLATOREMPTYREQUEST._serialized_end=20806
-  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_start=20808
-  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_end=20902
-  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_start=20904
-  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_end=21007
-  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_start=21009
-  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_end=21094
-  _TRANSLATORGETAXISOFFSETREQUEST._serialized_start=21096
-  _TRANSLATORGETAXISOFFSETREQUEST._serialized_end=21206
-  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_start=21208
-  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_end=21290
-  _DEVICESETSTORAGEREQUEST._serialized_start=21292
-  _DEVICESETSTORAGEREQUEST._serialized_end=21413
-  _DEVICEGETSTORAGEREQUEST._serialized_start=21415
-  _DEVICEGETSTORAGEREQUEST._serialized_end=21521
-  _DEVICESETSTORAGENUMBERREQUEST._serialized_start=21523
-  _DEVICESETSTORAGENUMBERREQUEST._serialized_end=21634
-  _DEVICESETSTORAGEBOOLREQUEST._serialized_start=21636
-  _DEVICESETSTORAGEBOOLREQUEST._serialized_end=21745
-  _DEVICESTORAGEREQUEST._serialized_start=21747
-  _DEVICESTORAGEREQUEST._serialized_end=21834
-  _DEVICESTORAGELISTKEYSREQUEST._serialized_start=21836
-  _DEVICESTORAGELISTKEYSREQUEST._serialized_end=21934
-  _DEVICESETUNITCONVERSIONSREQUEST._serialized_start=21937
-  _DEVICESETUNITCONVERSIONSREQUEST._serialized_end=22098
-  _CONVERSIONFACTOR._serialized_start=22100
-  _CONVERSIONFACTOR._serialized_end=22164
-  _OBJECTIVECHANGERREQUEST._serialized_start=22166
-  _OBJECTIVECHANGERREQUEST._serialized_end=22260
-  _OBJECTIVECHANGERCREATERESPONSE._serialized_start=22262
-  _OBJECTIVECHANGERCREATERESPONSE._serialized_end=22325
-  _OBJECTIVECHANGERCHANGEREQUEST._serialized_start=22328
-  _OBJECTIVECHANGERCHANGEREQUEST._serialized_end=22506
-  _OBJECTIVECHANGERGETCURRENTRESPONSE._serialized_start=22508
-  _OBJECTIVECHANGERGETCURRENTRESPONSE._serialized_end=22559
-  _PROCESSON._serialized_start=22561
-  _PROCESSON._serialized_end=22654
-  _PROCESSCONTROLLERSOURCE._serialized_start=22656
-  _PROCESSCONTROLLERSOURCE._serialized_end=22711
-  _SETPROCESSCONTROLLERSOURCE._serialized_start=22714
-  _SETPROCESSCONTROLLERSOURCE._serialized_end=22859
+  _INTREQUEST._serialized_start=304
+  _INTREQUEST._serialized_end=331
+  _BOOLRESPONSE._serialized_start=333
+  _BOOLRESPONSE._serialized_end=362
+  _DOUBLERESPONSE._serialized_start=364
+  _DOUBLERESPONSE._serialized_end=395
+  _DOUBLEARRAYRESPONSE._serialized_start=397
+  _DOUBLEARRAYRESPONSE._serialized_end=434
+  _INTRESPONSE._serialized_start=436
+  _INTRESPONSE._serialized_end=464
+  _STRINGRESPONSE._serialized_start=466
+  _STRINGRESPONSE._serialized_end=497
+  _STRINGARRAYRESPONSE._serialized_start=499
+  _STRINGARRAYRESPONSE._serialized_end=536
+  _AXISIDENTITY._serialized_start=539
+  _AXISIDENTITY._serialized_end=760
+  _AXISIDENTITY_AXISTYPE._serialized_start=713
+  _AXISIDENTITY_AXISTYPE._serialized_end=760
+  _DEVICEIDENTITY._serialized_start=763
+  _DEVICEIDENTITY._serialized_end=966
+  _FIRMWAREVERSION._serialized_start=968
+  _FIRMWAREVERSION._serialized_end=1030
+  _DEVICEIOINFO._serialized_start=1033
+  _DEVICEIOINFO._serialized_end=1171
+  _MEASUREMENT._serialized_start=1173
+  _MEASUREMENT._serialized_end=1232
+  _STREAMAXISDEFINITION._serialized_start=1234
+  _STREAMAXISDEFINITION._serialized_end=1296
+  _INVALIDPACKETEXCEPTIONDATA._serialized_start=1298
+  _INVALIDPACKETEXCEPTIONDATA._serialized_end=1358
+  _DEVICEADDRESSCONFLICTEXCEPTIONDATA._serialized_start=1360
+  _DEVICEADDRESSCONFLICTEXCEPTIONDATA._serialized_end=1422
+  _MOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_start=1424
+  _MOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_end=1522
+  _STREAMMOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_start=1524
+  _STREAMMOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_end=1598
+  _PVTMOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_start=1600
+  _PVTMOVEMENTINTERRUPTEDEXCEPTIONDATA._serialized_end=1671
+  _MOVEMENTFAILEDEXCEPTIONDATA._serialized_start=1673
+  _MOVEMENTFAILEDEXCEPTIONDATA._serialized_end=1766
+  _STREAMMOVEMENTFAILEDEXCEPTIONDATA._serialized_start=1768
+  _STREAMMOVEMENTFAILEDEXCEPTIONDATA._serialized_end=1837
+  _PVTMOVEMENTFAILEDEXCEPTIONDATA._serialized_start=1839
+  _PVTMOVEMENTFAILEDEXCEPTIONDATA._serialized_end=1905
+  _STREAMEXECUTIONEXCEPTIONDATA._serialized_start=1907
+  _STREAMEXECUTIONEXCEPTIONDATA._serialized_end=1973
+  _PVTEXECUTIONEXCEPTIONDATA._serialized_start=1976
+  _PVTEXECUTIONEXCEPTIONDATA._serialized_end=2104
+  _INVALIDPVTPOINT._serialized_start=2106
+  _INVALIDPVTPOINT._serialized_end=2153
+  _INVALIDRESPONSEEXCEPTIONDATA._serialized_start=2155
+  _INVALIDRESPONSEEXCEPTIONDATA._serialized_end=2203
+  _COMMANDFAILEDEXCEPTIONDATA._serialized_start=2206
+  _COMMANDFAILEDEXCEPTIONDATA._serialized_end=2389
+  _BINARYCOMMANDFAILEDEXCEPTIONDATA._serialized_start=2391
+  _BINARYCOMMANDFAILEDEXCEPTIONDATA._serialized_end=2448
+  _SETPERIPHERALSTATEEXCEPTIONDATA._serialized_start=2451
+  _SETPERIPHERALSTATEEXCEPTIONDATA._serialized_end=2588
+  _SETDEVICESTATEEXCEPTIONDATA._serialized_start=2591
+  _SETDEVICESTATEEXCEPTIONDATA._serialized_end=2844
+  _COMMANDTOOLONGEXCEPTIONDATA._serialized_start=2846
+  _COMMANDTOOLONGEXCEPTIONDATA._serialized_end=2949
+  _TESTREQUEST._serialized_start=2951
+  _TESTREQUEST._serialized_end=3037
+  _TESTRESPONSE._serialized_start=3039
+  _TESTRESPONSE._serialized_end=3072
+  _TESTRESPONSELONG._serialized_start=3074
+  _TESTRESPONSELONG._serialized_end=3111
+  _TESTEVENT._serialized_start=3113
+  _TESTEVENT._serialized_end=3138
+  _TOOLSLISTSERIALPORTSRESPONSE._serialized_start=3140
+  _TOOLSLISTSERIALPORTSRESPONSE._serialized_end=3185
+  _SETINTERNALMODEREQUEST._serialized_start=3187
+  _SETINTERNALMODEREQUEST._serialized_end=3225
+  _SETDEVICEDBSOURCEREQUEST._serialized_start=3227
+  _SETDEVICEDBSOURCEREQUEST._serialized_end=3300
+  _TOGGLEDEVICEDBSTOREREQUEST._serialized_start=3302
+  _TOGGLEDEVICEDBSTOREREQUEST._serialized_end=3373
+  _DEVICEDBFAILEDEXCEPTIONDATA._serialized_start=3375
+  _DEVICEDBFAILEDEXCEPTIONDATA._serialized_end=3418
+  _OPENINTERFACEREQUEST._serialized_start=3421
+  _OPENINTERFACEREQUEST._serialized_end=3716
+  _OPENINTERFACERESPONSE._serialized_start=3718
+  _OPENINTERFACERESPONSE._serialized_end=3763
+  _INTERFACEEMPTYREQUEST._serialized_start=3765
+  _INTERFACEEMPTYREQUEST._serialized_end=3810
+  _SETINTERFACETIMEOUTREQUEST._serialized_start=3812
+  _SETINTERFACETIMEOUTREQUEST._serialized_end=3879
+  _SETINTERFACECHECKSUMENABLEDREQUEST._serialized_start=3881
+  _SETINTERFACECHECKSUMENABLEDREQUEST._serialized_end=3959
+  _AXISEMPTYREQUEST._serialized_start=3961
+  _AXISEMPTYREQUEST._serialized_end=4031
+  _GENERICCOMMANDREQUEST._serialized_start=4034
+  _GENERICCOMMANDREQUEST._serialized_end=4165
+  _GENERICCOMMANDRESPONSE._serialized_start=4168
+  _GENERICCOMMANDRESPONSE._serialized_end=4368
+  _GENERICCOMMANDRESPONSECOLLECTION._serialized_start=4370
+  _GENERICCOMMANDRESPONSECOLLECTION._serialized_end=4471
+  _UNKNOWNRESPONSEEVENT._serialized_start=4474
+  _UNKNOWNRESPONSEEVENT._serialized_end=4694
+  _ALERTEVENT._serialized_start=4697
+  _ALERTEVENT._serialized_end=4828
+  _DISCONNECTEDEVENT._serialized_start=4830
+  _DISCONNECTEDEVENT._serialized_end=4946
+  _DEVICEIDENTIFYREQUEST._serialized_start=4948
+  _DEVICEIDENTIFYREQUEST._serialized_end=5074
+  _DEVICERENUMBERREQUEST._serialized_start=5076
+  _DEVICERENUMBERREQUEST._serialized_end=5144
+  _DEVICEDETECTREQUEST._serialized_start=5147
+  _DEVICEDETECTREQUEST._serialized_end=5333
+  _DEVICEDETECTREQUEST_DEVICETYPE._serialized_start=5288
+  _DEVICEDETECTREQUEST_DEVICETYPE._serialized_end=5333
+  _DEVICEDETECTRESPONSE._serialized_start=5335
+  _DEVICEDETECTRESPONSE._serialized_end=5374
+  _DEVICEHOMEREQUEST._serialized_start=5376
+  _DEVICEHOMEREQUEST._serialized_end=5472
+  _DEVICEWAITUNTILIDLEREQUEST._serialized_start=5474
+  _DEVICEWAITUNTILIDLEREQUEST._serialized_end=5584
+  _DEVICEMOVEREQUEST._serialized_start=5587
+  _DEVICEMOVEREQUEST._serialized_end=5923
+  _DEVICEMOVEREQUEST_MOVETYPE._serialized_start=5868
+  _DEVICEMOVEREQUEST_MOVETYPE._serialized_end=5923
+  _DEVICESTOPREQUEST._serialized_start=5925
+  _DEVICESTOPREQUEST._serialized_end=6021
+  _DEVICEONALLREQUEST._serialized_start=6023
+  _DEVICEONALLREQUEST._serialized_end=6090
+  _DEVICEONALLRESPONSE._serialized_start=6092
+  _DEVICEONALLRESPONSE._serialized_end=6139
+  _DEVICEGETWARNINGSREQUEST._serialized_start=6141
+  _DEVICEGETWARNINGSREQUEST._serialized_end=6234
+  _DEVICEGETWARNINGSRESPONSE._serialized_start=6236
+  _DEVICEGETWARNINGSRESPONSE._serialized_end=6278
+  _WAITTOCLEARWARNINGSREQUEST._serialized_start=6280
+  _WAITTOCLEARWARNINGSREQUEST._serialized_end=6400
+  _DEVICEGETALLDIGITALIOREQUEST._serialized_start=6402
+  _DEVICEGETALLDIGITALIOREQUEST._serialized_end=6492
+  _DEVICEGETALLDIGITALIORESPONSE._serialized_start=6494
+  _DEVICEGETALLDIGITALIORESPONSE._serialized_end=6541
+  _DEVICEGETALLANALOGIOREQUEST._serialized_start=6543
+  _DEVICEGETALLANALOGIOREQUEST._serialized_end=6632
+  _DEVICEGETALLANALOGIORESPONSE._serialized_start=6634
+  _DEVICEGETALLANALOGIORESPONSE._serialized_end=6680
+  _DEVICEGETDIGITALIOREQUEST._serialized_start=6682
+  _DEVICEGETDIGITALIOREQUEST._serialized_end=6793
+  _DEVICEGETANALOGIOREQUEST._serialized_start=6795
+  _DEVICEGETANALOGIOREQUEST._serialized_end=6905
+  _DEVICESETALLDIGITALOUTPUTSREQUEST._serialized_start=6907
+  _DEVICESETALLDIGITALOUTPUTSREQUEST._serialized_end=6996
+  _DEVICESETALLANALOGOUTPUTSREQUEST._serialized_start=6998
+  _DEVICESETALLANALOGOUTPUTSREQUEST._serialized_end=7086
+  _DEVICESETDIGITALOUTPUTREQUEST._serialized_start=7088
+  _DEVICESETDIGITALOUTPUTREQUEST._serialized_end=7196
+  _DEVICESETANALOGOUTPUTREQUEST._serialized_start=7198
+  _DEVICESETANALOGOUTPUTREQUEST._serialized_end=7305
+  _SETLOGOUTPUTREQUEST._serialized_start=7307
+  _SETLOGOUTPUTREQUEST._serialized_end=7361
+  _DEVICEGETSETTINGREQUEST._serialized_start=7363
+  _DEVICEGETSETTINGREQUEST._serialized_end=7471
+  _DEVICECONVERTSETTINGREQUEST._serialized_start=7474
+  _DEVICECONVERTSETTINGREQUEST._serialized_end=7622
+  _DEVICESETSETTINGREQUEST._serialized_start=7624
+  _DEVICESETSETTINGREQUEST._serialized_end=7747
+  _DEVICESETSETTINGSTRREQUEST._serialized_start=7749
+  _DEVICESETSETTINGSTRREQUEST._serialized_end=7861
+  _PREPARECOMMANDREQUEST._serialized_start=7864
+  _PREPARECOMMANDREQUEST._serialized_end=8022
+  _WAITTORESPONDREQUEST._serialized_start=8024
+  _WAITTORESPONDREQUEST._serialized_end=8101
+  _LOCKSTEPENABLEREQUEST._serialized_start=8103
+  _LOCKSTEPENABLEREQUEST._serialized_end=8205
+  _LOCKSTEPDISABLEREQUEST._serialized_start=8207
+  _LOCKSTEPDISABLEREQUEST._serialized_end=8321
+  _LOCKSTEPSTOPREQUEST._serialized_start=8323
+  _LOCKSTEPSTOPREQUEST._serialized_end=8434
+  _LOCKSTEPHOMEREQUEST._serialized_start=8436
+  _LOCKSTEPHOMEREQUEST._serialized_end=8547
+  _LOCKSTEPMOVEREQUEST._serialized_start=8550
+  _LOCKSTEPMOVEREQUEST._serialized_end=8903
+  _LOCKSTEPMOVEREQUEST_MOVETYPE._serialized_start=5868
+  _LOCKSTEPMOVEREQUEST_MOVETYPE._serialized_end=5923
+  _LOCKSTEPWAITUNTILIDLEREQUEST._serialized_start=8905
+  _LOCKSTEPWAITUNTILIDLEREQUEST._serialized_end=9030
+  _LOCKSTEPEMPTYREQUEST._serialized_start=9032
+  _LOCKSTEPEMPTYREQUEST._serialized_end=9119
+  _LOCKSTEPAXES._serialized_start=9121
+  _LOCKSTEPAXES._serialized_end=9199
+  _LOCKSTEPGETAXISNUMBERSRESPONSE._serialized_start=9201
+  _LOCKSTEPGETAXISNUMBERSRESPONSE._serialized_end=9247
+  _LOCKSTEPGETREQUEST._serialized_start=9249
+  _LOCKSTEPGETREQUEST._serialized_end=9348
+  _LOCKSTEPSETREQUEST._serialized_start=9351
+  _LOCKSTEPSETREQUEST._serialized_end=9485
+  _OSCILLOSCOPEADDSETTINGCHANNELREQUEST._serialized_start=9487
+  _OSCILLOSCOPEADDSETTINGCHANNELREQUEST._serialized_end=9594
+  _OSCILLOSCOPEADDIOCHANNELREQUEST._serialized_start=9596
+  _OSCILLOSCOPEADDIOCHANNELREQUEST._serialized_end=9704
+  _OSCILLOSCOPESTARTSTOPREQUEST._serialized_start=9706
+  _OSCILLOSCOPESTARTSTOPREQUEST._serialized_end=9813
+  _OSCILLOSCOPEREADRESPONSE._serialized_start=9815
+  _OSCILLOSCOPEREADRESPONSE._serialized_end=9859
+  _OSCILLOSCOPEDATAIDENTIFIER._serialized_start=9861
+  _OSCILLOSCOPEDATAIDENTIFIER._serialized_end=9906
+  _OSCILLOSCOPECAPTUREPROPERTIES._serialized_start=9908
+  _OSCILLOSCOPECAPTUREPROPERTIES._serialized_end=10035
+  _OSCILLOSCOPEDATAGETREQUEST._serialized_start=10037
+  _OSCILLOSCOPEDATAGETREQUEST._serialized_end=10096
+  _OSCILLOSCOPEDATAGETSAMPLETIMEREQUEST._serialized_start=10098
+  _OSCILLOSCOPEDATAGETSAMPLETIMEREQUEST._serialized_end=10182
+  _OSCILLOSCOPEDATAGETSAMPLESRESPONSE._serialized_start=10184
+  _OSCILLOSCOPEDATAGETSAMPLESRESPONSE._serialized_end=10234
+  _STREAMSETUPLIVEREQUEST._serialized_start=10236
+  _STREAMSETUPLIVEREQUEST._serialized_end=10344
+  _STREAMSETUPLIVECOMPOSITEREQUEST._serialized_start=10347
+  _STREAMSETUPLIVECOMPOSITEREQUEST._serialized_end=10510
+  _STREAMSETUPSTOREREQUEST._serialized_start=10513
+  _STREAMSETUPSTOREREQUEST._serialized_end=10665
+  _STREAMSETUPSTORECOMPOSITEREQUEST._serialized_start=10668
+  _STREAMSETUPSTORECOMPOSITEREQUEST._serialized_end=10875
+  _STREAMSETUPSTOREARBITRARYAXESREQUEST._serialized_start=10878
+  _STREAMSETUPSTOREARBITRARYAXESREQUEST._serialized_end=11049
+  _STREAMCALLREQUEST._serialized_start=11052
+  _STREAMCALLREQUEST._serialized_end=11184
+  _PVTPOINTREQUEST._serialized_start=11187
+  _PVTPOINTREQUEST._serialized_end=11524
+  _PVTPOINTREQUEST_TYPE._serialized_start=11500
+  _PVTPOINTREQUEST_TYPE._serialized_end=11524
+  _STREAMLINEREQUEST._serialized_start=11527
+  _STREAMLINEREQUEST._serialized_end=11788
+  _STREAMLINEREQUEST_TYPE._serialized_start=11500
+  _STREAMLINEREQUEST_TYPE._serialized_end=11524
+  _STREAMARCREQUEST._serialized_start=11791
+  _STREAMARCREQUEST._serialized_end=12292
+  _STREAMARCREQUEST_TYPE._serialized_start=11500
+  _STREAMARCREQUEST_TYPE._serialized_end=11524
+  _STREAMCIRCLEREQUEST._serialized_start=12295
+  _STREAMCIRCLEREQUEST._serialized_end=12643
+  _STREAMCIRCLEREQUEST_TYPE._serialized_start=11500
+  _STREAMCIRCLEREQUEST_TYPE._serialized_end=11524
+  _STREAMWAITDIGITALINPUTREQUEST._serialized_start=12646
+  _STREAMWAITDIGITALINPUTREQUEST._serialized_end=12786
+  _STREAMWAITANALOGINPUTREQUEST._serialized_start=12789
+  _STREAMWAITANALOGINPUTREQUEST._serialized_end=12947
+  _STREAMSETDIGITALOUTPUTREQUEST._serialized_start=12950
+  _STREAMSETDIGITALOUTPUTREQUEST._serialized_end=13090
+  _STREAMSETANALOGOUTPUTREQUEST._serialized_start=13093
+  _STREAMSETANALOGOUTPUTREQUEST._serialized_end=13232
+  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_start=13235
+  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_end=13363
+  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_start=13365
+  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_end=13486
+  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_start=13488
+  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_end=13608
+  _STREAMWAITREQUEST._serialized_start=13610
+  _STREAMWAITREQUEST._serialized_end=13727
+  _STREAMWAITUNTILIDLEREQUEST._serialized_start=13730
+  _STREAMWAITUNTILIDLEREQUEST._serialized_end=13858
+  _STREAMEMPTYREQUEST._serialized_start=13860
+  _STREAMEMPTYREQUEST._serialized_end=13950
+  _STREAMGETAXESRESPONSE._serialized_start=13952
+  _STREAMGETAXESRESPONSE._serialized_end=14035
+  _STREAMGETMAXSPEEDREQUEST._serialized_start=14037
+  _STREAMGETMAXSPEEDREQUEST._serialized_end=14147
+  _STREAMSETMAXSPEEDREQUEST._serialized_start=14150
+  _STREAMSETMAXSPEEDREQUEST._serialized_end=14279
+  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=14281
+  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=14408
+  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=14411
+  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=14575
+  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=14578
+  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=14706
+  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=14709
+  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=14875
+  _STREAMBUFFERGETCONTENTREQUEST._serialized_start=14877
+  _STREAMBUFFERGETCONTENTREQUEST._serialized_end=14978
+  _STREAMBUFFERGETCONTENTRESPONSE._serialized_start=14980
+  _STREAMBUFFERGETCONTENTRESPONSE._serialized_end=15034
+  _STREAMBUFFERERASEREQUEST._serialized_start=15036
+  _STREAMBUFFERERASEREQUEST._serialized_end=15132
+  _STREAMGENERICCOMMANDREQUEST._serialized_start=15134
+  _STREAMGENERICCOMMANDREQUEST._serialized_end=15250
+  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_start=15252
+  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_end=15371
+  _BINARYREPLYONLYEVENT._serialized_start=15373
+  _BINARYREPLYONLYEVENT._serialized_end=15472
+  _OPENBINARYINTERFACEREQUEST._serialized_start=15475
+  _OPENBINARYINTERFACEREQUEST._serialized_end=15662
+  _UNKNOWNBINARYRESPONSEEVENT._serialized_start=15664
+  _UNKNOWNBINARYRESPONSEEVENT._serialized_end=15769
+  _GENERICBINARYREQUEST._serialized_start=15772
+  _GENERICBINARYREQUEST._serialized_end=15902
+  _BINARYMESSAGE._serialized_start=15904
+  _BINARYMESSAGE._serialized_end=15974
+  _BINARYMESSAGECOLLECTION._serialized_start=15976
+  _BINARYMESSAGECOLLECTION._serialized_end=16058
+  _DEVICEEMPTYREQUEST._serialized_start=16060
+  _DEVICEEMPTYREQUEST._serialized_end=16118
+  _BINARYDEVICEIDENTITY._serialized_start=16121
+  _BINARYDEVICEIDENTITY._serialized_end=16466
+  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_start=16417
+  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_end=16466
+  _BINARYGENERICWITHUNITSREQUEST._serialized_start=16469
+  _BINARYGENERICWITHUNITSREQUEST._serialized_end=16622
+  _BINARYDEVICEHOMEREQUEST._serialized_start=16624
+  _BINARYDEVICEHOMEREQUEST._serialized_end=16718
+  _BINARYDEVICEMOVEREQUEST._serialized_start=16721
+  _BINARYDEVICEMOVEREQUEST._serialized_end=16939
+  _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_start=5868
+  _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_end=5905
+  _BINARYDEVICESTOPREQUEST._serialized_start=16941
+  _BINARYDEVICESTOPREQUEST._serialized_end=17035
+  _BINARYDEVICEDETECTREQUEST._serialized_start=17037
+  _BINARYDEVICEDETECTREQUEST._serialized_end=17112
+  _BINARYDEVICEDETECTRESPONSE._serialized_start=17114
+  _BINARYDEVICEDETECTRESPONSE._serialized_end=17159
+  _BINARYDEVICEGETSETTINGREQUEST._serialized_start=17161
+  _BINARYDEVICEGETSETTINGREQUEST._serialized_end=17261
+  _BINARYDEVICESETSETTINGREQUEST._serialized_start=17263
+  _BINARYDEVICESETSETTINGREQUEST._serialized_end=17378
+  _CUSTOMINTERFACEREADREQUEST._serialized_start=17380
+  _CUSTOMINTERFACEREADREQUEST._serialized_end=17430
+  _CUSTOMINTERFACEWRITEREQUEST._serialized_start=17432
+  _CUSTOMINTERFACEWRITEREQUEST._serialized_end=17500
+  _CUSTOMINTERFACEOPENRESPONSE._serialized_start=17502
+  _CUSTOMINTERFACEOPENRESPONSE._serialized_end=17553
+  _CUSTOMINTERFACECLOSEREQUEST._serialized_start=17555
+  _CUSTOMINTERFACECLOSEREQUEST._serialized_end=17629
+  _CANSETSTATEREQUEST._serialized_start=17631
+  _CANSETSTATEREQUEST._serialized_end=17718
+  _CANSETSTATEAXISRESPONSE._serialized_start=17720
+  _CANSETSTATEAXISRESPONSE._serialized_end=17781
+  _CANSETSTATEDEVICERESPONSE._serialized_start=17783
+  _CANSETSTATEDEVICERESPONSE._serialized_end=17895
+  _SETSTATEREQUEST._serialized_start=17897
+  _SETSTATEREQUEST._serialized_end=18002
+  _SERVOTUNINGREQUEST._serialized_start=18004
+  _SERVOTUNINGREQUEST._serialized_end=18094
+  _SERVOTUNINGPARAM._serialized_start=18096
+  _SERVOTUNINGPARAM._serialized_end=18143
+  _PARAMSETINFO._serialized_start=18145
+  _PARAMSETINFO._serialized_end=18248
+  _SETSERVOTUNINGREQUEST._serialized_start=18251
+  _SETSERVOTUNINGREQUEST._serialized_end=18409
+  _LOADPARAMSET._serialized_start=18411
+  _LOADPARAMSET._serialized_end=18521
+  _SETSERVOTUNINGPIDREQUEST._serialized_start=18524
+  _SETSERVOTUNINGPIDREQUEST._serialized_end=18665
+  _PIDTUNING._serialized_start=18667
+  _PIDTUNING._serialized_end=18754
+  _SETSIMPLETUNING._serialized_start=18757
+  _SETSIMPLETUNING._serialized_end=18951
+  _SIMPLETUNINGPARAMDEFINITION._serialized_start=18953
+  _SIMPLETUNINGPARAMDEFINITION._serialized_end=19053
+  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_start=19055
+  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_end=19164
+  _TRANSLATORCREATEREQUEST._serialized_start=19167
+  _TRANSLATORCREATEREQUEST._serialized_end=19316
+  _TRANSLATORCREATERESPONSE._serialized_start=19318
+  _TRANSLATORCREATERESPONSE._serialized_end=19367
+  _TRANSLATORAXISDEFINITION._serialized_start=19369
+  _TRANSLATORAXISDEFINITION._serialized_end=19448
+  _TRANSLATORDEFINITION._serialized_start=19451
+  _TRANSLATORDEFINITION._serialized_end=19612
+  _TRANSLATORCONFIG._serialized_start=19615
+  _TRANSLATORCONFIG._serialized_end=19787
+  _TRANSLATORAXISMAPPING._serialized_start=19789
+  _TRANSLATORAXISMAPPING._serialized_end=19853
+  _TRANSLATORAXISTRANSFORMATION._serialized_start=19855
+  _TRANSLATORAXISTRANSFORMATION._serialized_end=19981
+  _TRANSLATORTRANSLATEREQUEST._serialized_start=19983
+  _TRANSLATORTRANSLATEREQUEST._serialized_end=20049
+  _TRANSLATEMESSAGE._serialized_start=20051
+  _TRANSLATEMESSAGE._serialized_end=20124
+  _TRANSLATORTRANSLATERESPONSE._serialized_start=20126
+  _TRANSLATORTRANSLATERESPONSE._serialized_end=20233
+  _GCODESYNTAXEXCEPTIONDATA._serialized_start=20235
+  _GCODESYNTAXEXCEPTIONDATA._serialized_end=20299
+  _GCODEEXECUTIONEXCEPTIONDATA._serialized_start=20301
+  _GCODEEXECUTIONEXCEPTIONDATA._serialized_end=20368
+  _TRANSLATORFLUSHLIVEREQUEST._serialized_start=20370
+  _TRANSLATORFLUSHLIVEREQUEST._serialized_end=20446
+  _TRANSLATORFLUSHRESPONSE._serialized_start=20448
+  _TRANSLATORFLUSHRESPONSE._serialized_end=20491
+  _TRANSLATORCREATELIVEREQUEST._serialized_start=20494
+  _TRANSLATORCREATELIVEREQUEST._serialized_end=20638
+  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_start=20641
+  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_end=20786
+  _TRANSLATOREMPTYREQUEST._serialized_start=20788
+  _TRANSLATOREMPTYREQUEST._serialized_end=20835
+  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_start=20837
+  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_end=20931
+  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_start=20933
+  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_end=21036
+  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_start=21038
+  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_end=21123
+  _TRANSLATORGETAXISOFFSETREQUEST._serialized_start=21125
+  _TRANSLATORGETAXISOFFSETREQUEST._serialized_end=21235
+  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_start=21237
+  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_end=21319
+  _DEVICESETSTORAGEREQUEST._serialized_start=21321
+  _DEVICESETSTORAGEREQUEST._serialized_end=21442
+  _DEVICEGETSTORAGEREQUEST._serialized_start=21444
+  _DEVICEGETSTORAGEREQUEST._serialized_end=21550
+  _DEVICESETSTORAGENUMBERREQUEST._serialized_start=21552
+  _DEVICESETSTORAGENUMBERREQUEST._serialized_end=21663
+  _DEVICESETSTORAGEBOOLREQUEST._serialized_start=21665
+  _DEVICESETSTORAGEBOOLREQUEST._serialized_end=21774
+  _DEVICESTORAGEREQUEST._serialized_start=21776
+  _DEVICESTORAGEREQUEST._serialized_end=21863
+  _DEVICESTORAGELISTKEYSREQUEST._serialized_start=21865
+  _DEVICESTORAGELISTKEYSREQUEST._serialized_end=21963
+  _DEVICESETUNITCONVERSIONSREQUEST._serialized_start=21966
+  _DEVICESETUNITCONVERSIONSREQUEST._serialized_end=22127
+  _CONVERSIONFACTOR._serialized_start=22129
+  _CONVERSIONFACTOR._serialized_end=22193
+  _OBJECTIVECHANGERREQUEST._serialized_start=22195
+  _OBJECTIVECHANGERREQUEST._serialized_end=22289
+  _OBJECTIVECHANGERCREATERESPONSE._serialized_start=22291
+  _OBJECTIVECHANGERCREATERESPONSE._serialized_end=22354
+  _OBJECTIVECHANGERCHANGEREQUEST._serialized_start=22357
+  _OBJECTIVECHANGERCHANGEREQUEST._serialized_end=22535
+  _OBJECTIVECHANGERGETCURRENTRESPONSE._serialized_start=22537
+  _OBJECTIVECHANGERGETCURRENTRESPONSE._serialized_end=22588
+  _PROCESSON._serialized_start=22590
+  _PROCESSON._serialized_end=22683
+  _PROCESSCONTROLLERSOURCE._serialized_start=22685
+  _PROCESSCONTROLLERSOURCE._serialized_end=22740
+  _SETPROCESSCONTROLLERSOURCE._serialized_start=22743
+  _SETPROCESSCONTROLLERSOURCE._serialized_end=22888
 # @@protoc_insertion_point(module_scope)
```

### Comparing `zaber_motion-4.2.4/zaber_motion/protobufs/main_pb2.pyi` & `zaber_motion-4.2.5/zaber_motion/protobufs/main_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -247,14 +247,29 @@
     def __init__(
         self,
     ) -> None: ...
 
 global___EmptyRequest = EmptyRequest
 
 @typing_extensions.final
+class IntRequest(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    VALUE_FIELD_NUMBER: builtins.int
+    value: builtins.int
+    def __init__(
+        self,
+        *,
+        value: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["value", b"value"]) -> None: ...
+
+global___IntRequest = IntRequest
+
+@typing_extensions.final
 class BoolResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALUE_FIELD_NUMBER: builtins.int
     value: builtins.bool
     def __init__(
         self,
```

### Comparing `zaber_motion-4.2.4/zaber_motion/serialization.py` & `zaber_motion-4.2.5/zaber_motion/serialization.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/tools.py` & `zaber_motion-4.2.5/zaber_motion/tools.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion/units.py` & `zaber_motion-4.2.5/zaber_motion/units.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.4/zaber_motion.egg-info/PKG-INFO` & `zaber_motion-4.2.5/zaber_motion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaber-motion
-Version: 4.2.4
+Version: 4.2.5
 Summary: A library for communicating with Zaber devices
 Home-page: https://gitlab.com/ZaberTech/zaber-motion-lib
 Author: Zaber Technologies Inc.
 Author-email: contact@zaber.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `zaber_motion-4.2.4/zaber_motion.egg-info/SOURCES.txt` & `zaber_motion-4.2.5/zaber_motion.egg-info/SOURCES.txt`

 * *Files identical despite different names*


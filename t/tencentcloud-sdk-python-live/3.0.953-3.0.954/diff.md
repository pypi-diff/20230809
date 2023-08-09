# Comparing `tmp/tencentcloud-sdk-python-live-3.0.953.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.954.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.953.tar", last modified: Tue Aug  8 00:28:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.954.tar", last modified: Wed Aug  9 00:28:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.953.tar` & `tencentcloud-sdk-python-live-3.0.954.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/
--rw-r--r--   0 root         (0) root         (0)     1074 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20054 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   154723 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)   758493 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      506 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/tencentcloud_sdk_python_live.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      740 2023-08-08 00:28:00.000000 tencentcloud-sdk-python-live-3.0.953/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20054 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   157017 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)   761795 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      506 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/tencentcloud_sdk_python_live.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      740 2023-08-09 00:28:00.000000 tencentcloud-sdk-python-live-3.0.954/README.rst
```

### Comparing `tencentcloud-sdk-python-live-3.0.953/setup.py` & `tencentcloud-sdk-python-live-3.0.954/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-live',
-    install_requires=["tencentcloud-sdk-python-common==3.0.953"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.954"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Live SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-live-3.0.953/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.954/tencentcloud/live/v20180801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.953/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.954/tencentcloud/live/v20180801/live_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1142,15 +1142,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeAllStreamPlayInfoList(self, request):
-        """输入某个时间点（1分钟维度），查询该时间点所有流的下行信息。
+        """该接口为监控数据接口，数据采集及统计方式与计费数据不同，仅供运营分析使用，不能用于计费对账参考。
+        输入某个时间点（1分钟维度），查询该时间点所有流的下行信息。
 
         :param request: Request instance for DescribeAllStreamPlayInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeAllStreamPlayInfoListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeAllStreamPlayInfoListResponse`
 
         """
         try:
@@ -1211,15 +1212,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeCallbackRecordsList(self, request):
-        """用于查询回调事件。
+        """该接口为监控数据接口，数据采集及统计方式与计费数据不同，仅供运营分析使用，不能用于计费对账参考。
+        用于查询回调事件。
 
         :param request: Request instance for DescribeCallbackRecordsList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeCallbackRecordsListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeCallbackRecordsListResponse`
 
         """
         try:
@@ -1280,15 +1282,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeGroupProIspPlayInfoList(self, request):
-        """查询按省份和运营商分组的下行播放数据。
+        """该接口为监控数据接口，数据采集及统计方式与计费数据不同，仅供运营分析使用，不能用于计费对账参考。
+        查询按省份和运营商分组的下行播放数据。
 
         :param request: Request instance for DescribeGroupProIspPlayInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeGroupProIspPlayInfoListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeGroupProIspPlayInfoListResponse`
 
         """
         try:
@@ -1303,15 +1306,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeHttpStatusInfoList(self, request):
-        """查询某段时间内5分钟粒度的各播放http状态码的个数。
+        """该接口为监控数据接口，数据采集及统计方式与计费数据不同，仅供运营分析使用，不能用于计费对账参考。
+        查询某段时间内5分钟粒度的各播放http状态码的个数。
         备注：数据延迟1小时，如10:00-10:59点的数据12点才能查到。
 
         :param request: Request instance for DescribeHttpStatusInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeHttpStatusInfoListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeHttpStatusInfoListResponse`
 
         """
@@ -1534,15 +1538,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveDomainPlayInfoList(self, request):
-        """查询实时的域名维度下行播放数据，由于数据处理有耗时，接口默认查询4分钟前的准实时数据。
+        """该接口为监控数据接口，数据采集及统计方式与计费数据不同，仅供运营分析使用，不能用于计费对账参考。
+        查询实时的域名维度下行播放数据，由于数据处理有耗时，接口默认查询4分钟前的准实时数据。
 
         :param request: Request instance for DescribeLiveDomainPlayInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveDomainPlayInfoListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeLiveDomainPlayInfoListResponse`
 
         """
         try:
@@ -2076,15 +2081,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveStreamPushInfoList(self, request):
-        """查询所有实时流的推流信息，包括客户端IP，服务端IP，帧率，码率，域名，开始推流时间。
+        """该接口为监控数据接口，数据采集及统计方式与计费数据不同，仅供运营分析使用，不能用于计费对账参考。
+        查询所有实时流的推流信息，包括客户端IP，服务端IP，帧率，码率，域名，开始推流时间。
 
         :param request: Request instance for DescribeLiveStreamPushInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveStreamPushInfoListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeLiveStreamPushInfoListResponse`
 
         """
         try:
@@ -2200,15 +2206,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeLiveTranscodeDetailInfo(self, request):
-        """支持查询某天或某段时间的转码详细信息。由于转码数据量较大，如果查询时间跨度太长可能会拉不到数据，可以尝试将查询时间范围缩小些再重试。
+        """该接口为监控数据接口，数据采集及统计方式与计费数据不同，仅供运营分析使用，不能用于计费对账参考。
+        支持查询某天或某段时间的转码详细信息。由于转码数据量较大，如果查询时间跨度太长可能会拉不到数据，可以尝试将查询时间范围缩小些再重试。
 
         :param request: Request instance for DescribeLiveTranscodeDetailInfo.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLiveTranscodeDetailInfoRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeLiveTranscodeDetailInfoResponse`
 
         """
         try:
@@ -2456,16 +2463,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePlayErrorCodeDetailInfoList(self, request):
-        """查询下行播放错误码信息，某段时间内1分钟粒度的各http错误码出现的次数，包括4xx，5xx。
-
+        """该接口为监控数据接口，数据采集及统计方式与计费数据不同，仅供运营分析使用，不能用于计费对账参考。
+        查询下行播放错误码信息，某段时间内1分钟粒度的各http错误码出现的次数，包括4xx，5xx。
 
         :param request: Request instance for DescribePlayErrorCodeDetailInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribePlayErrorCodeDetailInfoListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribePlayErrorCodeDetailInfoListResponse`
 
         """
         try:
@@ -2480,15 +2487,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribePlayErrorCodeSumInfoList(self, request):
-        """查询下行播放错误码信息。
+        """该接口为监控数据接口，数据采集及统计方式与计费数据不同，仅供运营分析使用，不能用于计费对账参考。
+        查询下行播放错误码信息。
 
         :param request: Request instance for DescribePlayErrorCodeSumInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribePlayErrorCodeSumInfoListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribePlayErrorCodeSumInfoListResponse`
 
         """
         try:
@@ -2503,15 +2511,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProIspPlaySumInfoList(self, request):
-        """查询某段时间内每个国家地区每个省份每个运营商的平均每秒流量，总流量，总请求数信息。
+        """该接口为监控数据接口，数据采集及统计方式与计费数据不同，仅供运营分析使用，不能用于计费对账参考。
+        查询某段时间内每个国家地区每个省份每个运营商的平均每秒流量，总流量，总请求数信息。
 
         :param request: Request instance for DescribeProIspPlaySumInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeProIspPlaySumInfoListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeProIspPlaySumInfoListResponse`
 
         """
         try:
@@ -2526,15 +2535,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeProvinceIspPlayInfoList(self, request):
-        """查询某省份某运营商下行播放数据，包括带宽，流量，请求数，并发连接数信息。
+        """该接口为监控数据接口，数据采集及统计方式与计费数据不同，仅供运营分析使用，不能用于计费对账参考。
+        查询某省份某运营商下行播放数据，包括带宽，流量，请求数，并发连接数信息。
 
         :param request: Request instance for DescribeProvinceIspPlayInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeProvinceIspPlayInfoListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeProvinceIspPlayInfoListResponse`
 
         """
         try:
@@ -2671,15 +2681,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamDayPlayInfoList(self, request):
-        """查询天维度每条流的播放数据，包括总流量等。
+        """该接口为监控数据接口，数据采集及统计方式与计费数据不同，仅供运营分析使用，不能用于计费对账参考。
+        查询天维度每条流的播放数据，包括总流量等。
 
         :param request: Request instance for DescribeStreamDayPlayInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeStreamDayPlayInfoListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeStreamDayPlayInfoListResponse`
 
         """
         try:
@@ -2694,15 +2705,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamPlayInfoList(self, request):
-        """查询播放数据，支持按流名称查询详细播放数据，也可按播放域名查询详细总数据，数据延迟4分钟左右。
+        """该接口为监控数据接口，数据采集及统计方式与计费数据不同，仅供运营分析使用，不能用于计费对账参考。
+        查询播放数据，支持按流名称查询详细播放数据，也可按播放域名查询详细总数据，数据延迟4分钟左右。
 
         :param request: Request instance for DescribeStreamPlayInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeStreamPlayInfoListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeStreamPlayInfoListResponse`
 
         """
         try:
@@ -2717,15 +2729,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeStreamPushInfoList(self, request):
-        """查询流id的上行推流质量数据，包括音视频的帧率，码率，流逝时间，编码格式等。
+        """该接口为监控数据接口，数据采集及统计方式与计费数据不同，仅供运营分析使用，不能用于计费对账参考。
+        查询流id的上行推流质量数据，包括音视频的帧率，码率，流逝时间，编码格式等。
 
         :param request: Request instance for DescribeStreamPushInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeStreamPushInfoListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeStreamPushInfoListResponse`
 
         """
         try:
@@ -2786,15 +2799,16 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeTopClientIpSumInfoList(self, request):
-        """查询某段时间top n客户端ip汇总信息（暂支持top 1000）
+        """该接口为监控数据接口，数据采集及统计方式与计费数据不同，仅供运营分析使用，不能用于计费对账参考。
+        查询某段时间top n客户端ip汇总信息（暂支持top 1000）
 
         :param request: Request instance for DescribeTopClientIpSumInfoList.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeTopClientIpSumInfoListRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeTopClientIpSumInfoListResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-live-3.0.953/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.954/tencentcloud/live/v20180801/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7875,17 +7875,23 @@
 class DescribeGroupProIspPlayInfoListRequest(AbstractModel):
     """DescribeGroupProIspPlayInfoList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _StartTime: 起始时间点，格式为yyyy-mm-dd HH:MM:SS。
+        :param _StartTime: 起始时间点，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
         :type StartTime: str
-        :param _EndTime: 结束时间点，格式为yyyy-mm-dd HH:MM:SS
+        :param _EndTime: 结束时间点，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
 时间跨度在（0,3小时]，支持最近1个月数据查询。
         :type EndTime: str
         :param _PlayDomains: 播放域名，默认为不填，表示求总体数据。
         :type PlayDomains: list of str
         :param _ProvinceNames: 省份列表，默认不填，则返回各省份的数据。
         :type ProvinceNames: list of str
         :param _IspNames: 运营商列表，默认不填，则返回整个运营商的数据。
@@ -8011,20 +8017,23 @@
 class DescribeHttpStatusInfoListRequest(AbstractModel):
     """DescribeHttpStatusInfoList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _StartTime: 起始时间，北京时间，
-格式：yyyy-mm-dd HH:MM:SS。
+        :param _StartTime: 起始时间，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
         :type StartTime: str
-        :param _EndTime: 结束时间，北京时间，
-格式：yyyy-mm-dd HH:MM:SS。
-注：最大时间跨度支持1天，支持最近3个月的数据查询。
+        :param _EndTime: 结束时间，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
         :type EndTime: str
         :param _PlayDomains: 播放域名列表。
         :type PlayDomains: list of str
         """
         self._StartTime = None
         self._EndTime = None
         self._PlayDomains = None
@@ -12709,19 +12718,23 @@
 class DescribePlayErrorCodeDetailInfoListRequest(AbstractModel):
     """DescribePlayErrorCodeDetailInfoList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _StartTime: 起始时间，北京时间，
-格式：yyyy-mm-dd HH:MM:SS。
+        :param _StartTime: 起始时间，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
         :type StartTime: str
-        :param _EndTime: 结束时间，北京时间，
-格式：yyyy-mm-dd HH:MM:SS。
+        :param _EndTime: 结束时间，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
 注：EndTime 和 StartTime 只支持最近1天的数据查询。
         :type EndTime: str
         :param _Granularity: 查询粒度：
 1-1分钟粒度。
         :type Granularity: int
         :param _StatType: 是，可选值包括”4xx”,”5xx”，支持”4xx,5xx”等这种混合模式。
         :type StatType: str
@@ -13147,19 +13160,23 @@
 class DescribeProIspPlaySumInfoListRequest(AbstractModel):
     """DescribeProIspPlaySumInfoList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _StartTime: 起始时间，北京时间，
-格式：yyyy-mm-dd HH:MM:SS。
+        :param _StartTime: 起始时间，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
         :type StartTime: str
-        :param _EndTime: 结束时间，北京时间，
-格式：yyyy-mm-dd HH:MM:SS。
+        :param _EndTime: 结束时间，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
 注：EndTime 和 StartTime 只支持最近1天的数据查询。
         :type EndTime: str
         :param _StatType: 统计的类型，可选值：”Province”(省份)，”Isp”(运营商)，“CountryOrArea”(国家或地区)。
         :type StatType: str
         :param _PlayDomains: 播放域名列表，不填则为全部。
         :type PlayDomains: list of str
         :param _PageNum: 页号，范围是[1,1000]，默认值是1。
@@ -13405,19 +13422,23 @@
 class DescribeProvinceIspPlayInfoListRequest(AbstractModel):
     """DescribeProvinceIspPlayInfoList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _StartTime: 起始时间点，当前使用北京时间，
-例：2019-02-21 10:00:00。
+        :param _StartTime: 起始时间点，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
         :type StartTime: str
-        :param _EndTime: 结束时间点，当前使用北京时间，
-例：2019-02-21 12:00:00。
+        :param _EndTime: 结束时间点，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
 注：EndTime 和 StartTime 只支持最近1天的数据查询。
         :type EndTime: str
         :param _Granularity: 支持如下粒度：
 1：1分钟粒度（跨度不支持超过1天）
         :type Granularity: int
         :param _StatType: 统计指标类型：
 “Bandwidth”：带宽
@@ -14654,17 +14675,24 @@
 
     """
 
     def __init__(self):
         r"""
         :param _StreamName: 流名称。
         :type StreamName: str
-        :param _StartTime: 起始时间点，北京时间，格式为yyyy-mm-dd HH:MM:SS。
+        :param _StartTime: 起始时间点，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
         :type StartTime: str
-        :param _EndTime: 结束时间点，北京时间，格式为yyyy-mm-dd HH:MM:SS，支持查询最近7天数据，建议查询时间跨度在3小时之内。
+        :param _EndTime: 结束时间点，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
+支持查询最近7天数据，建议查询时间跨度在3小时之内。
         :type EndTime: str
         :param _PushDomain: 推流域名。
         :type PushDomain: str
         :param _AppName: 推流路径，与推流和播放地址中的AppName保持一致，默认为 live。
         :type AppName: str
         """
         self._StreamName = None
@@ -15084,17 +15112,23 @@
 class DescribeTopClientIpSumInfoListRequest(AbstractModel):
     """DescribeTopClientIpSumInfoList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _StartTime: 起始时间点，格式为yyyy-mm-dd HH:MM:SS。
+        :param _StartTime: 起始时间点，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
         :type StartTime: str
-        :param _EndTime: 结束时间点，格式为yyyy-mm-dd HH:MM:SS
+        :param _EndTime: 结束时间点，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
 时间跨度在[0,4小时]，支持最近1天数据查询。
         :type EndTime: str
         :param _PlayDomains: 播放域名，默认为不填，表示求总体数据。
         :type PlayDomains: list of str
         :param _PageNum: 页号，范围是[1,1000]，默认值是1。
         :type PageNum: int
         :param _PageSize: 每页个数，范围是[1,1000]，默认值是20。
@@ -16855,15 +16889,18 @@
 class HttpCodeValue(AbstractModel):
     """HTTP返回码数据信息
 
     """
 
     def __init__(self):
         r"""
-        :param _Time: 时间，格式：yyyy-mm-dd HH:MM:SS。
+        :param _Time: 时间，
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
         :type Time: str
         :param _Numbers: 次数。
         :type Numbers: int
         :param _Percentage: 占比。
         :type Percentage: float
         """
         self._Time = None
@@ -16913,15 +16950,17 @@
     """播放错误码信息
 
     """
 
     def __init__(self):
         r"""
         :param _Time: 数据时间点，
-格式：yyyy-mm-dd HH:MM:SS。
+使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
         :type Time: str
         :param _HttpStatusInfoList: 播放状态码详细信息。
         :type HttpStatusInfoList: list of HttpStatusInfo
         """
         self._Time = None
         self._HttpStatusInfoList = None
 
@@ -22178,15 +22217,17 @@
 class PushQualityData(AbstractModel):
     """某条流的推流质量详情数据。
 
     """
 
     def __init__(self):
         r"""
-        :param _Time: 数据时间，格式: %Y-%m-%d %H:%M:%S.%ms，精确到毫秒级。
+        :param _Time: 数据时间，使用UTC格式时间，
+例如：2019-01-08T10:00:00Z。
+注意：北京时间值为 UTC 时间值 + 8 小时，格式按照 ISO 8601 标准表示，详见 [ISO 日期格式说明](https://cloud.tencent.com/document/product/266/11732#I)。
         :type Time: str
         :param _PushDomain: 推流域名。
         :type PushDomain: str
         :param _AppName: 推流路径。
         :type AppName: str
         :param _ClientIp: 推流客户端 IP。
         :type ClientIp: str
```

### Comparing `tencentcloud-sdk-python-live-3.0.953/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.954/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.953'
+__version__ = '3.0.954'
```

### Comparing `tencentcloud-sdk-python-live-3.0.953/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.954/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.953/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.954/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.953
+Version: 3.0.954
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.953/README.rst` & `tencentcloud-sdk-python-live-3.0.954/README.rst`

 * *Files identical despite different names*


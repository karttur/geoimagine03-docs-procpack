---
layout: subprocess
categories: subprocess
title: DownloadSentinelRegion
processurl: subprocid-DownloadSentinelRegion
rootprocid: SentinelProcess
subprocid: DownloadSentinelRegion
author: thomasg
excerpt: Download Sentinel granule meta data
date: 2022-04-10
modified: 2022-04-10
comments: true
share: true
---


```
{
  "userproject": {
    "userid": "karttur",
    "projectid": "karttur",
    "tractid": "karttur",
    "siteid": "*",
    "plotid": "*",
    "system": "system"
  },
  "period": {
    "timestep": "static"
  },
  "process": [
    {
      "processid": "DownloadSentinelRegion",
      "parameters": {
        "copycomp": "systemregion",
        "tablesearchid": "regionid",
        "granuleoverlap": "0.1",
        "orbitdirection": "B",
        "platformname": "Sentinel-2",
        "prodtype": "S2MSI1C",
        "cloudmax": "30",
        "startdate": "20140401",
        "enddate": "20300101",
        "startdoy": "1",
        "enddoy": "365"
      },
      "srcpath": {
        "dat": "shp",
        "hdr": "shp",
        "volume": ""
      },
      "dstpath": {
        "dat": "zip",
        "hdr": "zip",
        "volume": ""
      }
    }
  ]
}
```

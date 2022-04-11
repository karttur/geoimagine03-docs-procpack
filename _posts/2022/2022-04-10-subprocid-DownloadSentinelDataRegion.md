---
layout: subprocess
categories: subprocess
title: DownloadSentinelDataRegion
processurl: subprocid-DownloadSentinelDataRegion
rootprocid: SentinelProcess
subprocid: DownloadSentinelDataRegion
author: thomasg
excerpt: Download Sentinel data
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
      "processid": "DownloadSentinelDataRegion",
      "parameters": {
        "tiles": "True",
        "orbitdirection": "B",
        "platformname": "Sentinel-2",
        "downloaded": "N",
        "prodtype": "S2MSI1C",
        "cloudmax": "30"
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

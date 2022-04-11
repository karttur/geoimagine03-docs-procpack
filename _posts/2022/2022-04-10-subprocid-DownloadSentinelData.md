---
layout: subprocess
categories: subprocess
title: DownloadSentinelData
processurl: subprocid-DownloadSentinelData
rootprocid: SentinelProcess
subprocid: DownloadSentinelData
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
      "processid": "DownloadSentinelData",
      "parameters": {
        "tiles": "True",
        "orbitdirection": "B",
        "platformname": "Sentinel-2",
        "downloaded": "N",
        "prodtype": "S2MSI1C",
        "cloudmax": "30"
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

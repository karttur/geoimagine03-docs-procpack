---
layout: subprocess
categories: subprocess
title: CheckModisRegion
processurl: subprocid-CheckModisRegion
rootprocid: MODISProc
subprocid: CheckModisRegion
author: thomasg
excerpt: Extracts the content of modis scenes>
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
      "processid": "CheckModisRegion",
      "parameters": {
        "product": "",
        "version": "",
        "checkdownloaded": "True",
        "checkexploded": "True"
      },
      "srcpath": {
        "dat": "",
        "hdr": "hdf",
        "volume": ""
      },
      "dstpath": {
        "dat": "",
        "hdr": "tif",
        "volume": ""
      }
    }
  ]
}
```

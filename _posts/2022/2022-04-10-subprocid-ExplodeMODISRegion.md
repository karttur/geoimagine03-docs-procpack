---
layout: subprocess
categories: subprocess
title: ExplodeMODISRegion
processurl: subprocid-ExplodeMODISRegion
rootprocid: MODISProc
subprocid: ExplodeMODISRegion
author: thomasg
excerpt: Extracts the content of modis scenes
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
      "processid": "ExplodeMODISRegion",
      "parameters": {
        "exploded": "False",
        "asscript": "True",
        "product": "",
        "version": ""
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

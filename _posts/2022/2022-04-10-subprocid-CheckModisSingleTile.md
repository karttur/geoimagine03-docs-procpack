---
layout: subprocess
categories: subprocess
title: CheckModisSingleTile
processurl: subprocid-CheckModisSingleTile
rootprocid: MODISProc
subprocid: CheckModisSingleTile
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
      "processid": "CheckModisSingleTile",
      "parameters": {
        "product": "",
        "version": "",
        "checkdownloaded": "True",
        "checkexploded": "True",
        "xtile": "",
        "ytile": ""
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

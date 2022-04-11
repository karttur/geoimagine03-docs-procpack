---
layout: subprocess
categories: subprocess
title: DownloadDataPool
processurl: subprocid-DownloadDataPool
rootprocid: MODISProc
subprocid: DownloadDataPool
author: thomasg
excerpt: Download MODIS tile data from MODIS datapool
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
      "processid": "DownloadDataPool",
      "parameters": {
        "product": "MCD43A4",
        "version": "006"
      },
      "dstpath": {
        "dat": "hdf",
        "hdr": "hdf",
        "volume": ""
      }
    }
  ]
}
```

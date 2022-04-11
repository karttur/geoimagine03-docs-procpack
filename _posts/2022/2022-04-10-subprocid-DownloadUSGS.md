---
layout: subprocess
categories: subprocess
title: DownloadUSGS
processurl: subprocid-DownloadUSGS
rootprocid: USGSProc
subprocid: DownloadUSGS
author: thomasg
excerpt: Download USGS data
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
      "processid": "DownloadUSGS",
      "parameters": {
        "remoteuser": "user",
        "password": "password",
        "searchdone": "False",
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

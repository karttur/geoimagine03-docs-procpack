---
layout: subprocess
categories: subprocess
title: DownloadCopernicus
processurl: subprocid-DownloadCopernicus
rootprocid: CopernicusProc
subprocid: DownloadCopernicus
author: thomasg
excerpt: Download Copernicus data
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
      "processid": "DownloadCopernicus",
      "parameters": {
        "serverurl": "gisco-services.ec.europa.eu",
        "remoteuser": "user",
        "password": "password",
        "searchdone": "False",
        "product": "",
        "version": ""
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

---
layout: subprocess
categories: subprocess
title: DownLoadModisPolar
processurl: subprocid-DownLoadModisPolar
rootprocid: ModisPolar
subprocid: DownLoadModisPolar
author: thomasg
excerpt: Download MODIS data from NSIDC
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
      "processid": "DownLoadModisPolar",
      "parameters": {
        "searchdone": "false",
        "remoteuser": "",
        "asscript": "True",
        "serverurl": "https://n5eil01u.ecs.nsidc.org",
        "downloaded": "N",
        "product": "MYD10A2",
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

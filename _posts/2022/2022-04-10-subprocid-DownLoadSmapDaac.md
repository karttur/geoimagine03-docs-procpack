---
layout: subprocess
categories: subprocess
title: DownLoadSmapDaac
processurl: subprocid-DownLoadSmapDaac
rootprocid: SmapProc
subprocid: DownLoadSmapDaac
author: thomasg
excerpt: Download SMAP data from DAAC
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
      "processid": "DownLoadSmapDaac",
      "parameters": {
        "remoteuser": "",
        "asscript": "True",
        "serverurl": "https://n5eil01u.ecs.nsidc.org",
        "searchdone": "False",
        "product": "SPL3SMP_E",
        "version": "002"
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

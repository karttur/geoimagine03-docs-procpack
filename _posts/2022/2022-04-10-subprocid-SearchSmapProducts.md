---
layout: subprocess
categories: subprocess
title: SearchSmapProducts
processurl: subprocid-SearchSmapProducts
rootprocid: SmapProc
subprocid: SearchSmapProducts
author: thomasg
excerpt: Access available files in DAAC holding
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
      "processid": "SearchSmapProducts",
      "parameters": {
        "product": "SPL3SMP_E",
        "version": "002",
        "serverurl": "https://n5eil01u.ecs.nsidc.org"
      },
      "dstpath": {
        "volume": ""
      }
    }
  ]
}
```

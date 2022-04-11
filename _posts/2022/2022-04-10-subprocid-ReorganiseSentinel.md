---
layout: subprocess
categories: subprocess
title: ReorganiseSentinel
processurl: subprocid-ReorganiseSentinel
rootprocid: SentinelProcess
subprocid: ReorganiseSentinel
author: thomasg
excerpt: Reorganize Sentinel tiles and granules
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
      "processid": "ReorganiseSentinel",
      "parameters": {
        "searchpath": "",
        "tiles": "True",
        "platformname": "Sentinel-2",
        "prodtype": "S2MSI1C"
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

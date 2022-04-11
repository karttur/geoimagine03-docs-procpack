---
layout: subprocess
categories: subprocess
title: FindGranuleTiles
processurl: subprocid-FindGranuleTiles
rootprocid: SentinelProcess
subprocid: FindGranuleTiles
author: thomasg
excerpt: Find mgrs tiles covered by granulue
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
      "processid": "FindGranuleTiles",
      "parameters": {
        "granuleoverlap": "0.1",
        "platformname": "Sentinel-2",
        "downloaded": "N",
        "prodtype": "GRD",
        "mgrsversion": "NGA",
        "cloudmax": "100"
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

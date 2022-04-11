---
layout: subprocess
categories: subprocess
title: CheckModisBands
processurl: subprocid-CheckModisBands
rootprocid: MODISProc
subprocid: CheckModisBands
author: thomasg
excerpt: Check MODIS organization
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
      "processid": "CheckModisBands",
      "parameters": {
        "organized": "N",
        "redundant": "N",
        "download": "N",
        "extract": "N"
      },
      "srccomp": [
        {
          "user_def_1": {}
        },
        {
          "user_def..n": {}
        }
      ],
      "srcpath": {
        "dat": "",
        "hdr": "tif",
        "volume": ""
      },
      "srcperiod": {
        "timestep": "allscenes"
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

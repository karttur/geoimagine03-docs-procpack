---
layout: subprocess
categories: subprocess
title: CheckModisScenes
processurl: subprocid-CheckModisScenes
rootprocid: MODISProc
subprocid: CheckModisScenes
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
      "processid": "CheckModisScenes",
      "parameters": {
        "redundant": "N"
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
        "hdr": "hdf",
        "volume": ""
      },
      "srcperiod": {
        "timestep": "allscenes"
      }
    }
  ]
}
```

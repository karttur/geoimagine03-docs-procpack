---
layout: subprocess
categories: subprocess
title: TractFromVector
processurl: subprocid-TractFromVector
rootprocid: ManageRegion
subprocid: TractFromVector
author: thomasg
excerpt: Define tract from extent
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
      "processid": "TractFromVector",
      "parameters": {
        "defaultregion": "",
        "tractid": "",
        "tracttitle": "",
        "tractlabel": "",
        "buffer": "0"
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
        "hdr": "shp",
        "volume": ""
      },
      "dstpath": {
        "volume": "",
        "hdr": "shp",
        "dat": ""
      }
    }
  ]
}
```

---
layout: subprocess
categories: subprocess
title: SiteFromVector
processurl: subprocid-SiteFromVector
rootprocid: ManageRegion
subprocid: SiteFromVector
author: thomasg
excerpt: Define site from extent
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
      "processid": "SiteFromVector",
      "parameters": {
        "tractid": "",
        "siteid": "",
        "sitetitle": "",
        "sitelabel": "",
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

---
layout: subprocess
categories: subprocess
title: MissingModisTiles
processurl: subprocid-MissingModisTiles
rootprocid: MODISProc
subprocid: MissingModisTiles
author: thomasg
excerpt: Copies closest neighboring tile to missing
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
      "processid": "MissingModisTiles",
      "parameters": {
        "product": "MCD43A4",
        "version": "006"
      },
      "srccomp": [
        {
          "user_def_1": {}
        },
        {
          "user_def..n": {}
        }
      ],
      "srcband": {
        "id": "",
        "layerid": "",
        "prefix": ""
      },
      "srcpath": {
        "dat": "",
        "hdr": "tif",
        "volume": ""
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

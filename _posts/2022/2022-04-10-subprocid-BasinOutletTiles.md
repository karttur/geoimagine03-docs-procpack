---
layout: subprocess
categories: subprocess
title: BasinOutletTiles
processurl: subprocid-BasinOutletTiles
rootprocid: BasinProc
subprocid: BasinOutletTiles
author: thomasg
excerpt: Refine pre-identified basin mouths in tiles data
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
      "processid": "BasinOutletTiles",
      "parameters": {
        "tiltmouths": "False",
        "grassdem": "DEM",
        "outlet": "MOUTH",
        "distill": "MOUTH",
        "clusteroutlet": "maximum",
        "basincelltrehshold": "-1",
        "watershed": "MFD",
        "memory": "300",
        "asscript": "True",
        "mosaic": "True"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        }
      ],
      "dstcopy": {
        "layerid": "auto",
        "prefix": "auto",
        "srccomp": "*",
        "suffix": "auto"
      },
      "dstpath": {
        "volume": ""
      }
    }
  ]
}
```

---
layout: subprocess
categories: subprocess
title: Grass1to1Tiles
processurl: subprocid-Grass1to1Tiles
rootprocid: GrassProc
subprocid: Grass1to1Tiles
author: thomasg
excerpt: Grass binding for tile processes 1 to 1
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
      "processid": "Grass1to1Tiles",
      "parameters": {
        "mosaic": "False",
        "asscript": "False",
        "regionlayer": "",
        "subparameter": ""
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
      "srcpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      },
      "dstcopy": {
        "cellnull": "auto",
        "celltype": "auto",
        "content": "",
        "dataunit": "auto",
        "layerid": "*",
        "masked": "N",
        "measure": "auto",
        "offsetadd": "0",
        "prefix": "",
        "product": "",
        "scalefac": "1",
        "source": "",
        "srccomp": "*",
        "suffix": ""
      },
      "dstpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      }
    }
  ]
}
```

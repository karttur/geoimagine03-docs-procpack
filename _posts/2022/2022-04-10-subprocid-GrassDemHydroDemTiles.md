---
layout: subprocess
categories: subprocess
title: GrassDemHydroDemTiles
processurl: subprocid-GrassDemHydroDemTiles
rootprocid: GrassDemProc
subprocid: GrassDemHydroDemTiles
author: thomasg
excerpt: Fill up dem pits
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
      "processid": "GrassDemHydroDemTiles",
      "parameters": {
        "superimpose": "True",
        "asscript": "True",
        "mosaic": "True",
        "flags": "",
        "size": "4",
        "mod": "4",
        "diffthreshold": "0.01",
        "query": "",
        "memory": "300",
        "tilesize": "1000",
        "tileoverlap": "10"
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
        "layerid": "*",
        "prefix": "*",
        "srccomp": "*"
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

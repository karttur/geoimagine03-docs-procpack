---
layout: subprocess
categories: subprocess
title: ExtractTilesPointVector
processurl: subprocid-ExtractTilesPointVector
rootprocid: Extract
subprocid: ExtractTilesPointVector
author: thomasg
excerpt: Extract raster data for listed coordinates
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
      "processid": "ExtractTilesPointVector",
      "parameters": {
        "kernelsize": "1",
        "mean": "True",
        "std": "True",
        "range": "True",
        "minimum": "True",
        "maximum": "True",
        "mode": "True"
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
        "ext": "csv",
        "layerid": "copy",
        "prefix": "copy",
        "srccomp": "*",
        "suffix": "copy"
      },
      "dstpath": {
        "volume": "",
        "hdr": "csv",
        "dat": ""
      }
    }
  ]
}
```

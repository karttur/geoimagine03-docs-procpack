---
layout: subprocess
categories: subprocess
title: NumpyDemRegion
processurl: subprocid-NumpyDemRegion
rootprocid: NumpyProc
subprocid: NumpyDemRegion
author: thomasg
excerpt: Generate DEM derivates
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
      "processid": "NumpyDemRegion",
      "parameters": {
        "mode": "slope",
        "trigonometric": "False",
        "algorithm": "default",
        "kernelform": "square",
        "kernelvalues": "equal",
        "standardize": "False",
        "palette": ""
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

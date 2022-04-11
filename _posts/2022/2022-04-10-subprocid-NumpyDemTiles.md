---
layout: subprocess
categories: subprocess
title: NumpyDemTiles
processurl: subprocid-NumpyDemTiles
rootprocid: NumpyProc
subprocid: NumpyDemTiles
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
      "processid": "NumpyDemTiles",
      "parameters": {
        "mode": "slope",
        "mosaic": "True",
        "radiuscsv": "1",
        "compute_edges": "True",
        "trigonometric": "False",
        "kernelform": "square",
        "kernelvalues": "equal",
        "standardize": "False",
        "tpithreshold": "5",
        "slopethreshold": "1",
        "dtpistd": "25",
        "btpistd": "50",
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
        "dataunit": "auto",
        "layerid": "auto",
        "prefix": "auto",
        "srccomp": "*",
        "suffix": "auto"
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

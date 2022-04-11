---
layout: subprocess
categories: subprocess
title: GdalDemTiles
processurl: subprocid-GdalDemTiles
rootprocid: DemProc
subprocid: GdalDemTiles
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
      "processid": "GdalDemTiles",
      "parameters": {
        "mode": "slope",
        "mosaic": "True",
        "radiuscsv": "1",
        "compute_edges": "False",
        "trigonometric": "False",
        "azimuth": "315",
        "altitude": "45",
        "zfac": "1",
        "algorithm": "default",
        "zero_for_flat": "True",
        "color_text_file": "",
        "palette": "",
        "asscript": "False"
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

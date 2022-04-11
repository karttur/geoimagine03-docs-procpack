---
layout: subprocess
categories: subprocess
title: GdalDemRegion
processurl: subprocid-GdalDemRegion
rootprocid: DemProc
subprocid: GdalDemRegion
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
      "processid": "GdalDemRegion",
      "parameters": {
        "mode": "slope",
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

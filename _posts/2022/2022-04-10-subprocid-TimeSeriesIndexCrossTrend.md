---
layout: subprocess
categories: subprocess
title: TimeSeriesIndexCrossTrend
processurl: subprocid-TimeSeriesIndexCrossTrend
rootprocid: TimeSeries
subprocid: TimeSeriesIndexCrossTrend
author: thomasg
excerpt: Index time-series cross trends
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
      "processid": "TimeSeriesIndexCrossTrend",
      "parameters": {
        "version": "1.3",
        "copycomp": "indexcrosstrend",
        "mirrorlag": "True",
        "maxlag": "6",
        "savelags": "-1",
        "normalize": "False",
        "standardize": "True",
        "naive": "False",
        "additive": "True",
        "yearfac": "1",
        "trend": "spline",
        "prefilterseason": "False",
        "kernel": "0",
        "forceseason": "True",
        "abs": "False",
        "xcrossobserved": "True",
        "xcrosstendency": "False",
        "xcrosseason": "False",
        "xcrossresidual": "False",
        "xcrosspearson": "True",
        "xcrosslag": "True"
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
      "dstpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      },
      "stats": {
        "id": "",
        "layerid": ""
      },
      "index": {
        "id": ""
      }
    }
  ]
}
```

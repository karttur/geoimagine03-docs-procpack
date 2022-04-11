---
layout: subprocess
categories: subprocess
title: TimeSeriesDecompose
processurl: subprocid-TimeSeriesDecompose
rootprocid: TimeSeries
subprocid: TimeSeriesDecompose
author: thomasg
excerpt: Time-series decomposition
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
      "processid": "TimeSeriesDecompose",
      "parameters": {
        "copycomp": "decomposets",
        "version": "1.3",
        "naive": "False",
        "yearfac": "1",
        "trend": "spline",
        "prefilterseason": "False",
        "kernel": "0",
        "forceseason": "True"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "decomp",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "decomp",
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
      }
    }
  ]
}
```

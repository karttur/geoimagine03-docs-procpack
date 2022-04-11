---
layout: subprocess
categories: subprocess
title: TimeSeriesImageCrossTrend
processurl: subprocid-TimeSeriesImageCrossTrend
rootprocid: TimeSeries
subprocid: TimeSeriesImageCrossTrend
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
      "processid": "TimeSeriesImageCrossTrend",
      "parameters": {
        "version": "1.3",
        "copycomp": "imagecrosstrend",
        "mirrorlag": "False",
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
          "user_def_1": {}
        },
        {
          "user_def..n": {}
        }
      ],
      "srcpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      },
      "dstcomp": [
        {
          "user_def_1": {
            "content": "xcorr",
            "layerid": "noeffect",
            "product": "",
            "source": "",
            "suffix": "auto"
          }
        },
        {
          "user_def..n": {
            "content": "xcorr",
            "layerid": "noeffect",
            "product": "",
            "source": "",
            "suffix": "auto"
          }
        }
      ],
      "dstpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      }
    }
  ]
}
```

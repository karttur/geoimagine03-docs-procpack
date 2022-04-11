---
layout: subprocess
categories: subprocess
title: TimeSeriesCorrelateLag
processurl: subprocid-TimeSeriesCorrelateLag
rootprocid: TimeSeries
subprocid: TimeSeriesCorrelateLag
author: thomasg
excerpt: Time-series correlation for lag
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
      "processid": "TimeSeriesCorrelateLag",
      "parameters": {
        "version": "1.3",
        "spatialforce": "False"
      },
      "srccomp": [
        {
          "user_def_1": {}
        },
        {
          "user_def..n": {}
        }
      ],
      "srcforce": {
        "content": "auto",
        "layerid": "*",
        "prefix": "*",
        "product": "*",
        "source": "*",
        "suffix": "*"
      },
      "srcpath": {
        "dat": "",
        "hdr": "tif",
        "volume": ""
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

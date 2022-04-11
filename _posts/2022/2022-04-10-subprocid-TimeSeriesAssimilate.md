---
layout: subprocess
categories: subprocess
title: TimeSeriesAssimilate
processurl: subprocid-TimeSeriesAssimilate
rootprocid: TimeSeries
subprocid: TimeSeriesAssimilate
author: thomasg
excerpt: Time Series Assimilate
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
      "processid": "TimeSeriesAssimilate",
      "parameters": {
        "version": "1.3",
        "maxthreshold": "0",
        "minthreshold": "0",
        "assimfrac": "1.0",
        "kernel": "0",
        "dstmin": "0",
        "dstmax": "100",
        "copycomp": "assimilate",
        "assimsuffix": "",
        "dstsuffix": "",
        "acceptdualresol": "True"
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
      "dstpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      }
    }
  ]
}
```

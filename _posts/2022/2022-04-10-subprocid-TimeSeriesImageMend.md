---
layout: subprocess
categories: subprocess
title: TimeSeriesImageMend
processurl: subprocid-TimeSeriesImageMend
rootprocid: TimeSeries
subprocid: TimeSeriesImageMend
author: thomasg
excerpt: Mend image timeseries data
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
      "processid": "TimeSeriesImageMend",
      "parameters": {
        "copycomp": "1to1",
        "version": "1.3",
        "method": "interpolate",
        "validfraction": "0.5"
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
      "dstcomp": [
        {
          "user_def_1": {
            "content": "src",
            "layerid": "*",
            "prefix": "*",
            "product": "src",
            "source": "src",
            "suffix": "*"
          }
        },
        {
          "user_def..n": {
            "content": "src",
            "layerid": "*",
            "prefix": "*",
            "product": "src",
            "source": "src",
            "suffix": "*"
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

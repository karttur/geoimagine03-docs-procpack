---
layout: subprocess
categories: subprocess
title: AutoCorrelate
processurl: subprocid-AutoCorrelate
rootprocid: TimeSeries
subprocid: AutoCorrelate
author: thomasg
excerpt: Ancillary time-series autocorrelation, outputs as many bands as maximum lags set (nlags) in the paramters
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
      "processid": "AutoCorrelate",
      "parameters": {
        "version": "1.3",
        "nlags": "0",
        "partial": "False",
        "resampleseasonal": "False",
        "mirror": "0",
        "copycomp": "autocorr"
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

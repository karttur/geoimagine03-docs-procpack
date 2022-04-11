---
layout: subprocess
categories: subprocess
title: TimeSeriesResmple
processurl: subprocid-TimeSeriesResmple
rootprocid: TimeSeries
subprocid: TimeSeriesResmple
author: thomasg
excerpt: Resample time series to other interval
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
      "processid": "TimeSeriesResmple",
      "parameters": {
        "version": "1.3",
        "group": "False",
        "method": "avg"
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
      "dstlayer": {
        "celltype": "auto",
        "content": "auto",
        "dataunit": "auto",
        "layerid": "auto",
        "offsetadd": "auto",
        "prefix": "auto",
        "scalefac": "auto",
        "suffix": "auto"
      },
      "dstpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      },
      "tarperiod": {
        "addons": "0",
        "endday": "31",
        "endmonth": "12",
        "endyear": "2100",
        "maxdaysaddons": "0",
        "seasonendday": "31",
        "seasonendmonth": "12",
        "seasonstartday": "1",
        "seasonstartmonth": "1",
        "startday": "1",
        "startmonth": "1",
        "startyear": "1900",
        "timestep": "static"
      }
    }
  ]
}
```

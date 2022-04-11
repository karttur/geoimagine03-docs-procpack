---
layout: subprocess
categories: subprocess
title: AutoCorrelate
processurl: subprocid-AutoCorrelate
rootprocid: TimeSeries
subprocid: AutoCorrelate
author: thomasg
excerpt: Ancillary time-series autocorrelation, outputs as many bands as maximum lags set (nlags) in the paramters
date: 2022-04-11
modified: 2022-04-11
comments: true
share: true
---

#### Complete json command structure (overriding defaults)
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
#### Required json command structure (accepting all defaults)
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
      "parameters": {},
      "srccomp": [
        {
          "user_def_1": {}
        },
        {
          "user_def..n": {}
        }
      ],
      "srcpath": {
        "hdr": "tif",
        "volume": ""
      },
      "dstpath": {
        "volume": "",
        "hdr": "tif"
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | version | text | False | 1.3 |
| process | parameters | nlags | integer | False | 0 |
| process | parameters | partial | boolean | False | False |
| process | parameters | resampleseasonal | boolean | False | False |
| process | parameters | mirror | integer | False | 0 |
| process | parameters | copycomp | text | False | autocorr |
| process | srccomp | * | element | False | * |
| process | srccomp | element | text | False | * |
| process | srccomp | parent | text | False | process |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | True | tif |
| process | srcpath | volume | text | True | --- |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | True | tif |
| process | dstpath | dat | text | False | --- |

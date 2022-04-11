---
layout: subprocess
categories: subprocess
title: TimeSeriesAssimilate
processurl: subprocid-TimeSeriesAssimilate
rootprocid: TimeSeries
subprocid: TimeSeriesAssimilate
author: thomasg
excerpt: Time Series Assimilate
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
      "processid": "TimeSeriesAssimilate",
      "parameters": {
        "dstmin": "0",
        "dstmax": "100",
        "assimsuffix": "",
        "dstsuffix": ""
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
        "volume": ""
      },
      "dstpath": {
        "volume": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | version | text | False | 1.3 |
| process | parameters | maxthreshold | real | False | 0 |
| process | parameters | minthreshold | real | False | 0 |
| process | parameters | assimfrac | real | False | 1.0 |
| process | parameters | kernel | text | False | 0 |
| process | parameters | dstmin | real | True | 0 |
| process | parameters | dstmax | real | True | 100 |
| process | parameters | copycomp | text | False | assimilate |
| process | parameters | assimsuffix | text | True | --- |
| process | parameters | dstsuffix | text | True | --- |
| process | parameters | acceptdualresol | boolean | False | True |
| process | srccomp | element | text | False | timeseries |
| process | srccomp | parent | text | False | process |
| process | srccomp | timeseries | element | True | --- |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | dat | text | False | --- |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | dat | text | False | --- |

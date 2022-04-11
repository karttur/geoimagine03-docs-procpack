---
layout: subprocess
categories: subprocess
title: TimeSeriesDecompose
processurl: subprocid-TimeSeriesDecompose
rootprocid: TimeSeries
subprocid: TimeSeriesDecompose
author: thomasg
excerpt: Time-series decomposition
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
      "processid": "TimeSeriesDecompose",
      "parameters": {},
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
        "hdr": "tif"
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
| process | parameters | copycomp | text | False | decomposets |
| process | parameters | version | text | False | 1.3 |
| process | parameters | naive | Boolean | False | False |
| process | parameters | yearfac | integer | False | 1 |
| process | parameters | trend | text | False | spline |
| process | parameters | prefilterseason | bool | False | False |
| process | parameters | kernel | text | False | 0 |
| process | parameters | forceseason | boolean | False | True |
| process | srccomp | * | element | True | * |
| process | srccomp | element | text | False | * |
| process | srccomp | parent | text | False | process |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | True | tif |
| process | srcpath | dat | text | False | --- |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | True | tif |
| process | dstpath | dat | text | False | --- |

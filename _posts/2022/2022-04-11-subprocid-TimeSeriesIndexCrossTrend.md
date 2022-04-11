---
layout: subprocess
categories: subprocess
title: TimeSeriesIndexCrossTrend
processurl: subprocid-TimeSeriesIndexCrossTrend
rootprocid: TimeSeries
subprocid: TimeSeriesIndexCrossTrend
author: thomasg
excerpt: Index time-series cross trends
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
      "processid": "TimeSeriesIndexCrossTrend",
      "parameters": {
        "version": "1.3",
        "copycomp": "indexcrosstrend",
        "mirrorlag": "True",
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
      "dstpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      },
      "stats": {
        "id": "",
        "layerid": ""
      },
      "index": {
        "id": ""
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
      "processid": "TimeSeriesIndexCrossTrend",
      "parameters": {
        "copycomp": "indexcrosstrend"
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
        "hdr": "tif"
      },
      "dstpath": {
        "volume": "",
        "hdr": "tif"
      },
      "stats": {
        "id": "",
        "layerid": ""
      },
      "index": {
        "id": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | version | text | False | 1.3 |
| process | parameters | copycomp | text | True | indexcrosstrend |
| process | parameters | mirrorlag | boolean | False | True |
| process | parameters | maxlag | integer | False | 6 |
| process | parameters | savelags | integer | False | -1 |
| process | parameters | normalize | Boolean | False | False |
| process | parameters | standardize | Boolean | False | True |
| process | parameters | naive | Boolean | False | False |
| process | parameters | additive | Boolean | False | True |
| process | parameters | yearfac | integer | False | 1 |
| process | parameters | trend | text | False | spline |
| process | parameters | prefilterseason | bool | False | False |
| process | parameters | kernel | text | False | 0 |
| process | parameters | forceseason | boolean | False | True |
| process | parameters | abs | boolean | False | False |
| process | parameters | xcrossobserved | boolean | False | True |
| process | parameters | xcrosstendency | boolean | False | False |
| process | parameters | xcrosseason | boolean | False | False |
| process | parameters | xcrossresidual | boolean | False | False |
| process | parameters | xcrosspearson | boolean | False | True |
| process | parameters | xcrosslag | boolean | False | True |
| process | srccomp | * | element | True | * |
| process | srccomp | parent | text | False | process |
| process | srccomp | element | text | False | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | True | tif |
| process | srcpath | dat | text | False | --- |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | True | tif |
| process | dstpath | dat | text | False | --- |
| process | stats | id | text | True | --- |
| process | stats | layerid | text | True | --- |
| process | index | id | text | True | --- |

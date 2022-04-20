---
layout: subprocess
categories: subprocess
title: TimeSeriesExtractMinMax
processurl: subprocid-TimeSeriesExtractMinMax
rootprocid: TimeSeries
subprocid: TimeSeriesExtractMinMax
author: thomasg
excerpt: Extract timesereies minimum and maximum
date: 2022-04-20
modified: 2022-04-20
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
      "processid": "TimeSeriesExtractMinMax",
      "parameters": {
        "version": "1.3",
        "min": "True",
        "max": "True"
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
        "dat": "",
        "hdr": "tif",
        "volume": ""
      },
      "dstpath": {
        "dat": "",
        "hdr": "tif",
        "volume": ""
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
      "processid": "TimeSeriesExtractMinMax",
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
        "hdr": "tif",
        "volume": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | version | text | False | 1.3 |
| process | parameters | min | boolean | False | True |
| process | parameters | max | boolean | False | True |
| process | srccomp | content | text | False | auto |
| process | srccomp | layerid | text | True | src |
| process | srccomp | masked | bool | False | N |
| process | srccomp | prefix | text | False | auto |
| process | srccomp | product | text | False | * |
| process | srccomp | source | text | False | * |
| process | srccomp | suffix | text | False | auto |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | True | tif |
| process | srcpath | volume | text | True | --- |
| process | dstpath | dat | text | False | --- |
| process | dstpath | hdr | text | True | tif |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | version | to be completed |
| process | parameters | min | to be completed |
| process | parameters | max | to be completed |
| process | srccomp | content | to be completed |
| process | srccomp | layerid | to be completed |
| process | srccomp | masked | to be completed |
| process | srccomp | prefix | to be completed |
| process | srccomp | product | to be completed |
| process | srccomp | source | to be completed |
| process | srccomp | suffix | to be completed |
| process | srcpath | dat | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | volume | to be completed |
| process | dstpath | dat | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | volume | to be completed |

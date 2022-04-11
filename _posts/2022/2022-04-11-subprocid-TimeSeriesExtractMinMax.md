---
layout: subprocess
categories: subprocess
title: TimeSeriesExtractMinMax
processurl: subprocid-TimeSeriesExtractMinMax
rootprocid: TimeSeries
subprocid: TimeSeriesExtractMinMax
author: thomasg
excerpt: Extract timesereies minimum and maximum
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

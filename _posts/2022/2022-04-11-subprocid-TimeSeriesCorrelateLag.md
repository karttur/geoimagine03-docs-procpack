---
layout: subprocess
categories: subprocess
title: TimeSeriesCorrelateLag
processurl: subprocid-TimeSeriesCorrelateLag
rootprocid: TimeSeries
subprocid: TimeSeriesCorrelateLag
author: thomasg
excerpt: Time-series correlation for lag
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
      "processid": "TimeSeriesCorrelateLag",
      "parameters": {
        "version": "1.3",
        "spatialforce": "False"
      },
      "srccomp": [
        {
          "user_def_1": {}
        },
        {
          "user_def..n": {}
        }
      ],
      "srcforce": {
        "content": "auto",
        "layerid": "*",
        "prefix": "*",
        "product": "*",
        "source": "*",
        "suffix": "*"
      },
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
      "processid": "TimeSeriesCorrelateLag",
      "parameters": {},
      "srccomp": [
        {
          "user_def_1": {}
        },
        {
          "user_def..n": {}
        }
      ],
      "srcforce": {
        "layerid": "*",
        "prefix": "*",
        "suffix": "*"
      },
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
| process | parameters | spatialforce | bool | False | False |
| process | srccomp | content | text | False | auto |
| process | srccomp | layerid | text | True | * |
| process | srccomp | masked | bool | False | N |
| process | srccomp | prefix | text | False | auto |
| process | srccomp | product | text | False | * |
| process | srccomp | source | text | False | * |
| process | srccomp | suffix | text | False | auto |
| process | srcforce | content | text | False | auto |
| process | srcforce | layerid | text | True | * |
| process | srcforce | prefix | text | True | * |
| process | srcforce | product | text | False | * |
| process | srcforce | source | text | False | * |
| process | srcforce | suffix | text | True | * |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | True | tif |
| process | srcpath | volume | text | True | --- |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | True | tif |
| process | dstpath | dat | text | False | --- |

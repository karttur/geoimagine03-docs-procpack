---
layout: subprocess
categories: subprocess
title: TimeSeriesResmple
processurl: subprocid-TimeSeriesResmple
rootprocid: TimeSeries
subprocid: TimeSeriesResmple
author: thomasg
excerpt: Resample time series to other interval
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
      "processid": "TimeSeriesResmple",
      "parameters": {
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
        "hdr": "tif"
      },
      "dstlayer": {},
      "dstpath": {
        "volume": "",
        "hdr": "tif"
      },
      "tarperiod": {}
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | version | text | False | 1.3 |
| process | parameters | group | bool | True | False |
| process | parameters | method | text | True | avg |
| process | srccomp | content | text | False | auto |
| process | srccomp | layerid | text | True | src |
| process | srccomp | masked | bool | False | False |
| process | srccomp | prefix | text | False | auto |
| process | srccomp | product | text | False | * |
| process | srccomp | source | text | False | * |
| process | srccomp | suffix | text | False | auto |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | True | tif |
| process | srcpath | dat | text | False | --- |
| process | dstlayer | celltype | text | False | auto |
| process | dstlayer | content | text | False | auto |
| process | dstlayer | dataunit | text | False | auto |
| process | dstlayer | layerid | text | False | auto |
| process | dstlayer | offsetadd | integer | False | auto |
| process | dstlayer | prefix | text | False | auto |
| process | dstlayer | scalefac | real | False | auto |
| process | dstlayer | suffix | text | False | auto |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | True | tif |
| process | dstpath | dat | text | False | --- |
| process | tarperiod | addons | integer | False | 0 |
| process | tarperiod | endday | integer | False | 31 |
| process | tarperiod | endmonth | integer | False | 12 |
| process | tarperiod | endyear | integer | False | 2100 |
| process | tarperiod | maxdaysaddons | integer | False | 0 |
| process | tarperiod | seasonendday | integer | False | 31 |
| process | tarperiod | seasonendmonth | integer | False | 12 |
| process | tarperiod | seasonstartday | integer | False | 1 |
| process | tarperiod | seasonstartmonth | integer | False | 1 |
| process | tarperiod | startday | integer | False | 1 |
| process | tarperiod | startmonth | integer | False | 1 |
| process | tarperiod | startyear | integer | False | 1900 |
| process | tarperiod | timestep | text | False | static |

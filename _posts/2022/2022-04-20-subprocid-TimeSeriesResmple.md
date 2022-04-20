---
layout: subprocess
categories: subprocess
title: TimeSeriesResmple
processurl: subprocid-TimeSeriesResmple
rootprocid: TimeSeries
subprocid: TimeSeriesResmple
author: thomasg
excerpt: Resample time series to other interval
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

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | version | to be completed |
| process | parameters | group | to be completed |
| process | parameters | method | to be completed |
| process | srccomp | content | to be completed |
| process | srccomp | layerid | to be completed |
| process | srccomp | masked | to be completed |
| process | srccomp | prefix | to be completed |
| process | srccomp | product | to be completed |
| process | srccomp | source | to be completed |
| process | srccomp | suffix | to be completed |
| process | srcpath | volume | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | dat | to be completed |
| process | dstlayer | celltype | to be completed |
| process | dstlayer | content | to be completed |
| process | dstlayer | dataunit | to be completed |
| process | dstlayer | layerid | to be completed |
| process | dstlayer | offsetadd | to be completed |
| process | dstlayer | prefix | to be completed |
| process | dstlayer | scalefac | to be completed |
| process | dstlayer | suffix | to be completed |
| process | dstpath | volume | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | dat | to be completed |
| process | tarperiod | addons | added timesteps at start and end |
| process | tarperiod | endday | day of month of last data point |
| process | tarperiod | endmonth | month of last data point |
| process | tarperiod | endyear | year of last data point |
| process | tarperiod | maxdaysaddons | Maximum number of days allowed for adding to start and end |
| process | tarperiod | seasonendday | Last day of month of seasonal data |
| process | tarperiod | seasonendmonth | last month of seasonal data |
| process | tarperiod | seasonstartday | First day of month of seasonal data |
| process | tarperiod | seasonstartmonth | first month of seasonal data |
| process | tarperiod | startday | day of month of first data point |
| process | tarperiod | startmonth | month of first data point |
| process | tarperiod | startyear | year of first data point |
| process | tarperiod | timestep | Type of time series (loosely based on Pandas) |

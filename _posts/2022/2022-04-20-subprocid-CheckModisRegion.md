---
layout: subprocess
categories: subprocess
title: CheckModisRegion
processurl: subprocid-CheckModisRegion
rootprocid: MODISProc
subprocid: CheckModisRegion
author: thomasg
excerpt: Extracts the content of modis scenes>
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
      "processid": "CheckModisRegion",
      "parameters": {
        "product": "",
        "version": "",
        "checkdownloaded": "True",
        "checkexploded": "True"
      },
      "srcpath": {
        "dat": "",
        "hdr": "hdf",
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
      "processid": "CheckModisRegion",
      "parameters": {
        "product": "",
        "version": ""
      },
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
| process | parameters | product | text | True | --- |
| process | parameters | version | text | True | --- |
| process | parameters | checkdownloaded | boolean | False | True |
| process | parameters | checkexploded | boolean | False | True |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | False | hdf |
| process | srcpath | volume | text | True | --- |
| process | dstpath | dat | text | False | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | product | to be completed |
| process | parameters | version | to be completed |
| process | parameters | checkdownloaded | to be completed |
| process | parameters | checkexploded | to be completed |
| process | srcpath | dat | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | volume | to be completed |
| process | dstpath | dat | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | volume | to be completed |

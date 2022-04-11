---
layout: subprocess
categories: subprocess
title: ExplodeMODISRegion
processurl: subprocid-ExplodeMODISRegion
rootprocid: MODISProc
subprocid: ExplodeMODISRegion
author: thomasg
excerpt: Extracts the content of modis scenes
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
      "processid": "ExplodeMODISRegion",
      "parameters": {
        "exploded": "False",
        "asscript": "True",
        "product": "",
        "version": ""
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
      "processid": "ExplodeMODISRegion",
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
| process | parameters | exploded | bool | False | False |
| process | parameters | asscript | bool | False | True |
| process | parameters | product | text | True | --- |
| process | parameters | version | text | True | --- |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | False | hdf |
| process | srcpath | volume | text | True | --- |
| process | dstpath | dat | text | False | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | volume | text | True | --- |

---
layout: subprocess
categories: subprocess
title: CheckModisScenes
processurl: subprocid-CheckModisScenes
rootprocid: MODISProc
subprocid: CheckModisScenes
author: thomasg
excerpt: Check MODIS organization
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
      "processid": "CheckModisScenes",
      "parameters": {
        "redundant": "N"
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
        "hdr": "hdf",
        "volume": ""
      },
      "srcperiod": {
        "timestep": "allscenes"
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
      "processid": "CheckModisScenes",
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
        "volume": ""
      },
      "srcperiod": {}
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | redundant | bool | False | N |
| process | srccomp | content | text | True | original |
| process | srccomp | layerid | text | False | * |
| process | srccomp | masked | bool | False | N |
| process | srccomp | prefix | text | False | * |
| process | srccomp | product | text | False | * |
| process | srccomp | source | text | False | * |
| process | srccomp | suffix | text | False | * |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | False | hdf |
| process | srcpath | volume | text | True | --- |
| process | srcperiod | timestep | text | False | allscenes |

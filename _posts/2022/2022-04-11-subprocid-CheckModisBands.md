---
layout: subprocess
categories: subprocess
title: CheckModisBands
processurl: subprocid-CheckModisBands
rootprocid: MODISProc
subprocid: CheckModisBands
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
      "processid": "CheckModisBands",
      "parameters": {
        "organized": "N",
        "redundant": "N",
        "download": "N",
        "extract": "N"
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
      "srcperiod": {
        "timestep": "allscenes"
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
      "processid": "CheckModisBands",
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
      "srcperiod": {},
      "dstpath": {
        "volume": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | organized | bool | False | N |
| process | parameters | redundant | bool | False | N |
| process | parameters | download | bool | False | N |
| process | parameters | extract | bool | False | N |
| process | srccomp | content | text | True | original |
| process | srccomp | layerid | text | False | * |
| process | srccomp | masked | bool | False | N |
| process | srccomp | prefix | text | False | * |
| process | srccomp | product | text | False | * |
| process | srccomp | source | text | False | * |
| process | srccomp | suffix | text | False | * |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | volume | text | True | --- |
| process | srcperiod | timestep | text | False | allscenes |
| process | dstpath | dat | text | False | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | volume | text | True | --- |

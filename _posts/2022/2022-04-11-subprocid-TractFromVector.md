---
layout: subprocess
categories: subprocess
title: TractFromVector
processurl: subprocid-TractFromVector
rootprocid: ManageRegion
subprocid: TractFromVector
author: thomasg
excerpt: Define tract from extent
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
      "processid": "TractFromVector",
      "parameters": {
        "defaultregion": "",
        "tractid": "",
        "tracttitle": "",
        "tractlabel": "",
        "buffer": "0"
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
        "hdr": "shp",
        "volume": ""
      },
      "dstpath": {
        "volume": "",
        "hdr": "shp",
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
      "processid": "TractFromVector",
      "parameters": {
        "defaultregion": "",
        "tractid": "",
        "tracttitle": ""
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
| process | parameters | defaultregion | text | True | --- |
| process | parameters | tractid | text | True | --- |
| process | parameters | tracttitle | text | True | --- |
| process | parameters | tractlabel | text | False | --- |
| process | parameters | buffer | float | False | 0 |
| process | srccomp | element | text | False | process |
| process | srccomp | parent | text | False | process |
| process | srccomp | srctractextent | element | True | --- |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | False | shp |
| process | srcpath | volume | text | True | --- |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | shp |
| process | dstpath | dat | text | False | --- |

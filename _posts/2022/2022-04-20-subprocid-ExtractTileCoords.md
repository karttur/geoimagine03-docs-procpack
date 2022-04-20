---
layout: subprocess
categories: subprocess
title: ExtractTileCoords
processurl: subprocid-ExtractTileCoords
rootprocid: ManageRegion
subprocid: ExtractTileCoords
author: thomasg
excerpt: Extract tile coordinates
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
      "processid": "ExtractTileCoords",
      "parameters": {
        "centroid": "True",
        "mgrs": "MGRS",
        "gzd": "GZD",
        "utmzone": "ZONE",
        "wrspath": "PATH",
        "wrsrow": "ROW",
        "wrsmode": "MODE",
        "wrs": "2"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "vector",
            "layerid": "vector",
            "prefix": "vector",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "vector",
            "layerid": "vector",
            "prefix": "vector",
            "product": "",
            "source": "",
            "suffix": ""
          }
        }
      ],
      "srcpath": {
        "dat": "shp",
        "hdr": "shp",
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
      "processid": "ExtractTileCoords",
      "parameters": {
        "centroid": "True"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "vector",
            "layerid": "vector",
            "prefix": "vector",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "vector",
            "layerid": "vector",
            "prefix": "vector",
            "product": "",
            "source": "",
            "suffix": ""
          }
        }
      ],
      "srcpath": {
        "volume": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | centroid | bool | True | True |
| process | parameters | mgrs | text | False | MGRS |
| process | parameters | gzd | text | False | GZD |
| process | parameters | utmzone | text | False | ZONE |
| process | parameters | wrspath | text | False | PATH |
| process | parameters | wrsrow | text | False | ROW |
| process | parameters | wrsmode | text | False | MODE |
| process | parameters | wrs | integer | False | 2 |
| process | srccomp | * | element | True | * |
| process | srccomp | element | text | False | * |
| process | srccomp | parent | text | False | process |
| process | srcpath | dat | text | False | shp |
| process | srcpath | hdr | text | False | shp |
| process | srcpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | centroid | to be completed |
| process | parameters | mgrs | to be completed |
| process | parameters | gzd | to be completed |
| process | parameters | utmzone | to be completed |
| process | parameters | wrspath | to be completed |
| process | parameters | wrsrow | to be completed |
| process | parameters | wrsmode | to be completed |
| process | parameters | wrs | to be completed |
| process | srccomp | * | to be completed |
| process | srccomp | element | to be completed |
| process | srccomp | parent | to be completed |
| process | srcpath | dat | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | volume | to be completed |

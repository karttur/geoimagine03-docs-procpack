---
layout: subprocess
categories: subprocess
title: GrassDemReInterpolateTiles
processurl: subprocid-GrassDemReInterpolateTiles
rootprocid: GrassDemProc
subprocid: GrassDemReInterpolateTiles
author: thomasg
excerpt: Fill up dem pits
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
      "processid": "GrassDemReInterpolateTiles",
      "parameters": {
        "asscript": "True",
        "mosaic": "True",
        "flags": "4",
        "ew_res": "0",
        "ns_res": "0",
        "overlap": "3",
        "tension": "40",
        "tilesize": "1000",
        "tileoverlap": "10"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        }
      ],
      "srcpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      },
      "dstcopy": {
        "layerid": "*",
        "prefix": "*",
        "srccomp": "*"
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
      "processid": "GrassDemReInterpolateTiles",
      "parameters": {},
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        }
      ],
      "srcpath": {
        "volume": ""
      },
      "dstcopy": {
        "layerid": "*",
        "prefix": "*",
        "srccomp": "*"
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
| process | parameters | asscript | boolean | False | True |
| process | parameters | mosaic | text | False | True |
| process | parameters | flags | text | False | 4 |
| process | parameters | ew_res | float | False | 0 |
| process | parameters | ns_res | float | False | 0 |
| process | parameters | overlap | integer | False | 3 |
| process | parameters | tension | float | False | 40 |
| process | parameters | tilesize | integer | False | 1000 |
| process | parameters | tileoverlap | integer | False | 10 |
| process | srccomp | * | element | True | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcopy | layerid | text | True | * |
| process | dstcopy | prefix | text | True | * |
| process | dstcopy | srccomp | text | True | * |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | dat | text | False | --- |

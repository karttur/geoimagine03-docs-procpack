---
layout: subprocess
categories: subprocess
title: NumpyGeomorphologyTiles
processurl: subprocid-NumpyGeomorphologyTiles
rootprocid: NumpyProc
subprocid: NumpyGeomorphologyTiles
author: thomasg
excerpt: Extract Geomorphology from multilayers
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
      "processid": "NumpyGeomorphologyTiles",
      "parameters": {
        "mode": "weiss",
        "standardize": "False",
        "slopethreshold": "1",
        "tpithreshold": "5",
        "mosaic": "True",
        "radiuscsv": "1,3",
        "compute_edges": "True",
        "palette": ""
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
        "dataunit": "auto",
        "layerid": "auto",
        "prefix": "auto",
        "srccomp": "*",
        "suffix": "auto"
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
      "processid": "NumpyGeomorphologyTiles",
      "parameters": {
        "mode": "weiss"
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
        "volume": ""
      },
      "dstcopy": {
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
| process | parameters | mode | text | True | weiss |
| process | parameters | standardize | boolean | False | False |
| process | parameters | slopethreshold | float | False | 1 |
| process | parameters | tpithreshold | float | False | 5 |
| process | parameters | mosaic | boolean | False | True |
| process | parameters | radiuscsv | text | False | 1,3 |
| process | parameters | compute_edges | boolean | False | True |
| process | parameters | palette | text | False | --- |
| process | srccomp | * | element | True | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcopy | dataunit | text | False | auto |
| process | dstcopy | layerid | text | False | auto |
| process | dstcopy | prefix | text | False | auto |
| process | dstcopy | srccomp | text | True | * |
| process | dstcopy | suffix | text | False | auto |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | mode | to be completed |
| process | parameters | standardize | Standardize or not. |
| process | parameters | slopethreshold | slope threshold |
| process | parameters | tpithreshold | TPI threshold |
| process | parameters | mosaic | to be completed |
| process | parameters | radiuscsv | radius sizes separated with commas |
| process | parameters | compute_edges | to be completed |
| process | parameters | palette | Palette. |
| process | srccomp | * | link for source composition |
| process | srcpath | volume | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | dat | to be completed |
| process | dstcopy | dataunit | unknown hint |
| process | dstcopy | layerid | unknown hint |
| process | dstcopy | prefix | unknown hint |
| process | dstcopy | srccomp | unknown hint |
| process | dstcopy | suffix | unknown hint |
| process | dstpath | volume | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | dat | to be completed |

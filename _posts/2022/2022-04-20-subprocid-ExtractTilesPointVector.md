---
layout: subprocess
categories: subprocess
title: ExtractTilesPointVector
processurl: subprocid-ExtractTilesPointVector
rootprocid: Extract
subprocid: ExtractTilesPointVector
author: thomasg
excerpt: Extract raster data for listed coordinates
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
      "processid": "ExtractTilesPointVector",
      "parameters": {
        "kernelsize": "1",
        "mean": "True",
        "std": "True",
        "range": "True",
        "minimum": "True",
        "maximum": "True",
        "mode": "True"
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
        "ext": "csv",
        "layerid": "copy",
        "prefix": "copy",
        "srccomp": "*",
        "suffix": "copy"
      },
      "dstpath": {
        "volume": "",
        "hdr": "csv",
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
      "processid": "ExtractTilesPointVector",
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
        "volume": "",
        "hdr": "tif"
      },
      "dstcopy": {
        "srccomp": "*"
      },
      "dstpath": {
        "volume": "",
        "hdr": "csv"
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | kernelsize | integer | False | 1 |
| process | parameters | mean | boolean | False | True |
| process | parameters | std | boolean | False | True |
| process | parameters | range | boolean | False | True |
| process | parameters | minimum | boolean | False | True |
| process | parameters | maximum | boolean | False | True |
| process | parameters | mode | boolean | False | True |
| process | srccomp | * | element | True | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | True | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcopy | ext | text | False | csv |
| process | dstcopy | layerid | text | False | copy |
| process | dstcopy | prefix | text | False | copy |
| process | dstcopy | srccomp | text | True | * |
| process | dstcopy | suffix | text | False | copy |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | True | csv |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | kernelsize | to be completed |
| process | parameters | mean | to be completed |
| process | parameters | std | to be completed |
| process | parameters | range | to be completed |
| process | parameters | minimum | to be completed |
| process | parameters | maximum | to be completed |
| process | parameters | mode | to be completed |
| process | srccomp | * | link for source composition |
| process | srcpath | volume | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | dat | to be completed |
| process | dstcopy | ext | File typae for savning extracted raster stats |
| process | dstcopy | layerid | unknown hint |
| process | dstcopy | prefix | unknown hint |
| process | dstcopy | srccomp | unknown hint |
| process | dstcopy | suffix | unknown hint |
| process | dstpath | volume | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | dat | to be completed |

---
layout: subprocess
categories: subprocess
title: MosaicAdjacentTiles
processurl: subprocid-MosaicAdjacentTiles
rootprocid: Tiling
subprocid: MosaicAdjacentTiles
author: thomasg
excerpt: Expand tiles by mosaic adjacent tiles
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
      "processid": "MosaicAdjacentTiles",
      "parameters": {
        "version": "1.3",
        "asscript": "False",
        "fillnodata": "False",
        "fillmaxdist": "10",
        "fillsmooth": "0",
        "overlay": "mean",
        "tr_xres": "0",
        "tr_yres": "0",
        "resample": "near",
        "overlap": "101"
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
        "srccomp": "*",
        "suffix": "auto"
      },
      "dstpath": {
        "volume": "",
        "hdr": "vrt",
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
      "processid": "MosaicAdjacentTiles",
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
        "srccomp": "*",
        "suffix": "auto"
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
| process | parameters | version | text | False | 1.3 |
| process | parameters | asscript | boolean | False | False |
| process | parameters | fillnodata | boolean | False | False |
| process | parameters | fillmaxdist | integer | False | 10 |
| process | parameters | fillsmooth | integer | False | 0 |
| process | parameters | overlay | text | False | mean |
| process | parameters | tr_xres | real | False | 0 |
| process | parameters | tr_yres | real | False | 0 |
| process | parameters | resample | text | False | near |
| process | parameters | overlap | integer | False | 101 |
| process | srccomp | * | element | True | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcopy | layerid | text | True | * |
| process | dstcopy | srccomp | text | True | * |
| process | dstcopy | suffix | text | True | auto |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | vrt |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | version | to be completed |
| process | parameters | asscript | to be completed |
| process | parameters | fillnodata | to be completed |
| process | parameters | fillmaxdist | The maximum distance (in pixels) for interpolated filling |
| process | parameters | fillsmooth | The number of 3x3 average filter smoothing iterations to run after filling. |
| process | parameters | overlay | to be completed |
| process | parameters | tr_xres | to be completed |
| process | parameters | tr_yres | to be completed |
| process | parameters | resample | to be completed |
| process | parameters | overlap | edge overlap in cells |
| process | srccomp | * | link for source composition |
| process | srcpath | volume | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | dat | to be completed |
| process | dstcopy | layerid | unknown hint |
| process | dstcopy | srccomp | unknown hint |
| process | dstcopy | suffix | unknown hint |
| process | dstpath | volume | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | dat | to be completed |

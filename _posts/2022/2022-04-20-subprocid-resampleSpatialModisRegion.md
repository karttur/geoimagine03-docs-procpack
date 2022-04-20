---
layout: subprocess
categories: subprocess
title: resampleSpatialModisRegion
processurl: subprocid-resampleSpatialModisRegion
rootprocid: MODISProc
subprocid: resampleSpatialModisRegion
author: thomasg
excerpt: Tile regional SMAP data to fit modis
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
      "processid": "resampleSpatialModisRegion",
      "parameters": {
        "version": "1.3",
        "asscript": "True",
        "epsg": "6842",
        "xres": "463.313",
        "yres": "463.313",
        "resample": "near",
        "copycomp": "1to1",
        "suffix": "copy",
        "celltype": "auto"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "region",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": "",
            "system": "smap"
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "region",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": "",
            "system": "smap"
          }
        }
      ],
      "srcpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
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
      "processid": "resampleSpatialModisRegion",
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
| process | parameters | asscript | boolean | False | True |
| process | parameters | epsg | integer | False | 6842 |
| process | parameters | xres | real | False | 463.313 |
| process | parameters | yres | real | False | 463.313 |
| process | parameters | resample | text | False | near |
| process | parameters | copycomp | text | False | 1to1 |
| process | parameters | suffix | text | False | copy |
| process | parameters | celltype | text | False | auto |
| process | srccomp | element | text | False | * |
| process | srccomp | parent | text | False | process |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | dat | text | False | --- |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | version | to be completed |
| process | parameters | asscript | to be completed |
| process | parameters | epsg | to be completed |
| process | parameters | xres | to be completed |
| process | parameters | yres | to be completed |
| process | parameters | resample | to be completed |
| process | parameters | copycomp | to be completed |
| process | parameters | suffix | to be completed |
| process | parameters | celltype | to be completed |
| process | srccomp | element | to be completed |
| process | srccomp | parent | to be completed |
| process | srcpath | volume | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | dat | to be completed |
| process | dstpath | volume | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | dat | to be completed |

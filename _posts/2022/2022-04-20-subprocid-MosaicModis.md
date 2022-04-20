---
layout: subprocess
categories: subprocess
title: MosaicModis
processurl: subprocid-MosaicModis
rootprocid: MODISProc
subprocid: MosaicModis
author: thomasg
excerpt: Mosaic mdois raster tiles to region
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
      "processid": "MosaicModis",
      "parameters": {
        "version": "1.3",
        "overlay": "mean",
        "t_epsg": "0",
        "xres": "0",
        "yres": "0",
        "resample": "near",
        "celltype": "auto",
        "export": "False",
        "movieframes": "False",
        "copycomp": "1to1"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "region",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "region",
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
      "processid": "MosaicModis",
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
| process | parameters | overlay | text | False | mean |
| process | parameters | t_epsg | integer | False | 0 |
| process | parameters | xres | real | False | 0 |
| process | parameters | yres | real | False | 0 |
| process | parameters | resample | text | False | near |
| process | parameters | celltype | text | False | auto |
| process | parameters | export | bool | False | False |
| process | parameters | movieframes | bool | False | False |
| process | parameters | copycomp | text | False | 1to1 |
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
| process | parameters | overlay | to be completed |
| process | parameters | t_epsg | to be completed |
| process | parameters | xres | to be completed |
| process | parameters | yres | to be completed |
| process | parameters | resample | to be completed |
| process | parameters | celltype | to be completed |
| process | parameters | export | to be completed |
| process | parameters | movieframes | to be completed |
| process | parameters | copycomp | to be completed |
| process | srccomp | element | to be completed |
| process | srccomp | parent | to be completed |
| process | srcpath | volume | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | dat | to be completed |
| process | dstpath | volume | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | dat | to be completed |

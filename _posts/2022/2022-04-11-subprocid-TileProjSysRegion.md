---
layout: subprocess
categories: subprocess
title: TileProjSysRegion
processurl: subprocid-TileProjSysRegion
rootprocid: Tiling
subprocid: TileProjSysRegion
author: thomasg
excerpt: Tile regional data
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
      "processid": "TileProjSysRegion",
      "parameters": {
        "version": "1.3",
        "asscript": "False",
        "src_defregid": "",
        "tr_xres": "463.313",
        "tr_yres": "463.313",
        "resample": "near",
        "celltype": "auto",
        "srcnodata": "-222",
        "dstnodata": "-222",
        "errorthreshold": "0"
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
      "processid": "TileProjSysRegion",
      "parameters": {
        "src_defregid": "",
        "tr_xres": "463.313",
        "tr_yres": "463.313"
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
        "layerid": "*",
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
| process | parameters | version | text | False | 1.3 |
| process | parameters | asscript | boolean | False | False |
| process | parameters | src_defregid | text | True | --- |
| process | parameters | tr_xres | real | True | 463.313 |
| process | parameters | tr_yres | real | True | 463.313 |
| process | parameters | resample | text | False | near |
| process | parameters | celltype | text | False | auto |
| process | parameters | srcnodata | integer | False | -222 |
| process | parameters | dstnodata | integer | False | -222 |
| process | parameters | errorthreshold | real | False | 0 |
| process | srccomp | * | element | True | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcopy | layerid | text | True | * |
| process | dstcopy | srccomp | text | True | * |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | dat | text | False | --- |

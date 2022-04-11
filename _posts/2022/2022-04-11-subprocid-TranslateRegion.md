---
layout: subprocess
categories: subprocess
title: TranslateRegion
processurl: subprocid-TranslateRegion
rootprocid: Translate
subprocid: TranslateRegion
author: thomasg
excerpt: Translate regional data
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
      "processid": "TranslateRegion",
      "parameters": {
        "version": "1.3",
        "asscript": "False",
        "dstEPSG": "0",
        "xoff": "0",
        "yoff": "0",
        "xsize": "0",
        "ysize": "0",
        "tr_xres": "0.0",
        "tr_yres": "0.0",
        "resample": "near",
        "autofitextent": "True",
        "src_min": "0.0",
        "src_max": "0.0",
        "dst_min": "0.0",
        "dst_max": "0.0",
        "exponent": "0.0",
        "unscale": "False",
        "dst_ulx": "0.0",
        "dst_uly": "0.0",
        "dst_lrx": "0.0",
        "dst_lry": "0.0",
        "nodata": "-22.22",
        "celltype": "auto"
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
        "srccomp": "*",
        "layerid": "*"
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
      "processid": "TranslateRegion",
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
        "srccomp": "*",
        "layerid": "*"
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
| process | parameters | dstEPSG | integer | False | 0 |
| process | parameters | xoff | integer | False | 0 |
| process | parameters | yoff | integer | False | 0 |
| process | parameters | xsize | integer | False | 0 |
| process | parameters | ysize | integer | False | 0 |
| process | parameters | tr_xres | real | False | 0.0 |
| process | parameters | tr_yres | real | False | 0.0 |
| process | parameters | resample | text | False | near |
| process | parameters | autofitextent | boolean | False | True |
| process | parameters | src_min | real | False | 0.0 |
| process | parameters | src_max | real | False | 0.0 |
| process | parameters | dst_min | real | False | 0.0 |
| process | parameters | dst_max | real | False | 0.0 |
| process | parameters | exponent | real | False | 0.0 |
| process | parameters | unscale | boolean | False | False |
| process | parameters | dst_ulx | real | False | 0.0 |
| process | parameters | dst_uly | real | False | 0.0 |
| process | parameters | dst_lrx | real | False | 0.0 |
| process | parameters | dst_lry | real | False | 0.0 |
| process | parameters | nodata | real | False | -22.22 |
| process | parameters | celltype | text | False | auto |
| process | srccomp | * | element | True | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcopy | srccomp | text | True | * |
| process | dstcopy | layerid | text | True | * |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | dat | text | False | --- |
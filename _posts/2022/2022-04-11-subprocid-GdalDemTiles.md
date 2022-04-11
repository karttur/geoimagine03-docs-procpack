---
layout: subprocess
categories: subprocess
title: GdalDemTiles
processurl: subprocid-GdalDemTiles
rootprocid: DemProc
subprocid: GdalDemTiles
author: thomasg
excerpt: Generate DEM derivates
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
      "processid": "GdalDemTiles",
      "parameters": {
        "mode": "slope",
        "mosaic": "True",
        "radiuscsv": "1",
        "compute_edges": "False",
        "trigonometric": "False",
        "azimuth": "315",
        "altitude": "45",
        "zfac": "1",
        "algorithm": "default",
        "zero_for_flat": "True",
        "color_text_file": "",
        "palette": "",
        "asscript": "False"
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
      "processid": "GdalDemTiles",
      "parameters": {
        "mode": "slope"
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
| process | parameters | mode | text | True | slope |
| process | parameters | mosaic | boolean | False | True |
| process | parameters | radiuscsv | text | False | 1 |
| process | parameters | compute_edges | boolean | False | False |
| process | parameters | trigonometric | boolean | False | False |
| process | parameters | azimuth | integer | False | 315 |
| process | parameters | altitude | integer | False | 45 |
| process | parameters | zfac | float | False | 1 |
| process | parameters | algorithm | text | False | default |
| process | parameters | zero_for_flat | boolean | False | True |
| process | parameters | color_text_file | text | False | --- |
| process | parameters | palette | text | False | --- |
| process | parameters | asscript | boolean | False | False |
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

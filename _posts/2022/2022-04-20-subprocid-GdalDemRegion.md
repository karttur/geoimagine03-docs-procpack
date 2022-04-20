---
layout: subprocess
categories: subprocess
title: GdalDemRegion
processurl: subprocid-GdalDemRegion
rootprocid: DemProc
subprocid: GdalDemRegion
author: thomasg
excerpt: Generate DEM derivates
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
      "processid": "GdalDemRegion",
      "parameters": {
        "mode": "slope",
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
      "processid": "GdalDemRegion",
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
| process | parameters | compute_edges | to be completed |
| process | parameters | trigonometric | Trigonometric measure for slope and azimuth or not. |
| process | parameters | azimuth | azimuth value for hillshading |
| process | parameters | altitude | altitude value for hillshading |
| process | parameters | zfac | z factor for hillshading |
| process | parameters | algorithm | Algorithm for slope |
| process | parameters | zero_for_flat | flat=0 if true, otherwise -9999 |
| process | parameters | color_text_file | full path to color text file |
| process | parameters | palette | to be completed |
| process | parameters | asscript | to be completed |
| process | srccomp | * | link for source composition |
| process | srcpath | volume | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | dat | to be completed |
| process | dstcopy | layerid | unknown hint |
| process | dstcopy | prefix | unknown hint |
| process | dstcopy | srccomp | unknown hint |
| process | dstcopy | suffix | unknown hint |
| process | dstpath | volume | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | dat | to be completed |

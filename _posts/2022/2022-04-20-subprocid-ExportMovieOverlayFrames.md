---
layout: subprocess
categories: subprocess
title: ExportMovieOverlayFrames
processurl: subprocid-ExportMovieOverlayFrames
rootprocid: Export
subprocid: ExportMovieOverlayFrames
author: thomasg
excerpt: Convert 2 sets of exported images to movie frames with baselayer and overlayer
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
      "processid": "ExportMovieOverlayFrames",
      "parameters": {
        "overwriteshade": "False",
        "overwritelayout": "False",
        "name": "default",
        "basewidth": "0",
        "basecrop": "",
        "overlaywidth": "0",
        "gravity": "northeast",
        "geomx": "0",
        "geomy": "0",
        "emboss": "KARTTUR",
        "embossdims": "",
        "embossptsize": "0",
        "asscript": "True",
        "vector": "NA"
      },
      "srccomp": [
        {
          "user_def_1": {}
        },
        {
          "user_def..n": {}
        }
      ],
      "srcpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      },
      "dstcopy": {
        "srccomp": "*",
        "layerid": "copy",
        "prefix": "copy",
        "suffix": "copy"
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
      "processid": "ExportMovieOverlayFrames",
      "parameters": {
        "basewidth": "0",
        "basecrop": "",
        "overlaywidth": "0",
        "emboss": "KARTTUR",
        "embossdims": "",
        "embossptsize": "0"
      },
      "srccomp": [
        {
          "user_def_1": {}
        },
        {
          "user_def..n": {}
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
        "hdr": "tif"
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | overwriteshade | boolean | False | False |
| process | parameters | overwritelayout | boolean | False | False |
| process | parameters | name | text | False | default |
| process | parameters | basewidth | integer | True | 0 |
| process | parameters | basecrop | text | True | --- |
| process | parameters | overlaywidth | integer | True | 0 |
| process | parameters | gravity | text | False | northeast |
| process | parameters | geomx | integer | False | 0 |
| process | parameters | geomy | integer | False | 0 |
| process | parameters | emboss | text | True | KARTTUR |
| process | parameters | embossdims | text | True | --- |
| process | parameters | embossptsize | integer | True | 0 |
| process | parameters | asscript | bool | False | True |
| process | parameters | vector | text | False | NA |
| process | srccomp | * | element | True | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | True | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcopy | srccomp | text | True | * |
| process | dstcopy | layerid | text | False | copy |
| process | dstcopy | prefix | text | False | copy |
| process | dstcopy | suffix | text | False | copy |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | True | tif |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | overwriteshade | to be completed |
| process | parameters | overwritelayout | to be completed |
| process | parameters | name | to be completed |
| process | parameters | basewidth | to be completed |
| process | parameters | basecrop | to be completed |
| process | parameters | overlaywidth | to be completed |
| process | parameters | gravity | to be completed |
| process | parameters | geomx | to be completed |
| process | parameters | geomy | to be completed |
| process | parameters | emboss | to be completed |
| process | parameters | embossdims | to be completed |
| process | parameters | embossptsize | to be completed |
| process | parameters | asscript | to be completed |
| process | parameters | vector | to be completed |
| process | srccomp | * | link for source composition |
| process | srcpath | volume | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | dat | to be completed |
| process | dstcopy | srccomp | unknown hint |
| process | dstcopy | layerid | unknown hint |
| process | dstcopy | prefix | unknown hint |
| process | dstcopy | suffix | unknown hint |
| process | dstpath | volume | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | dat | to be completed |

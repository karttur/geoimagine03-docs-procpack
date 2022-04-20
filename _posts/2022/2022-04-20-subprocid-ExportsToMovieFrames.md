---
layout: subprocess
categories: subprocess
title: ExportsToMovieFrames
processurl: subprocid-ExportsToMovieFrames
rootprocid: Export
subprocid: ExportsToMovieFrames
author: thomasg
excerpt: Convert exported images to movie frames
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
      "processid": "ExportsToMovieFrames",
      "parameters": {
        "overwriteshade": "False",
        "overwritelayout": "False",
        "name": "default",
        "width": "0",
        "crop": "",
        "border": "0",
        "bordercolor": "black",
        "emboss": "KARTTUR",
        "embossdims": "",
        "embossptsize": "",
        "asscript": "True",
        "vectoroverlay": ""
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
        "layerid": "copy",
        "prefix": "copy",
        "srccomp": "*",
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
      "processid": "ExportsToMovieFrames",
      "parameters": {
        "width": "0",
        "emboss": "KARTTUR",
        "embossdims": "",
        "embossptsize": ""
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
| process | parameters | width | integer | True | 0 |
| process | parameters | crop | text | False | --- |
| process | parameters | border | integer | False | 0 |
| process | parameters | bordercolor | text | False | black |
| process | parameters | emboss | text | True | KARTTUR |
| process | parameters | embossdims | text | True | --- |
| process | parameters | embossptsize | integer | True | --- |
| process | parameters | asscript | bool | False | True |
| process | parameters | vectoroverlay | text | False | --- |
| process | srccomp | * | element | True | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | True | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcopy | layerid | text | False | copy |
| process | dstcopy | prefix | text | False | copy |
| process | dstcopy | srccomp | text | True | * |
| process | dstcopy | suffix | text | False | copy |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | True | tif |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | overwriteshade | to be completed |
| process | parameters | overwritelayout | to be completed |
| process | parameters | name | to be completed |
| process | parameters | width | to be completed |
| process | parameters | crop | to be completed |
| process | parameters | border | to be completed |
| process | parameters | bordercolor | to be completed |
| process | parameters | emboss | to be completed |
| process | parameters | embossdims | to be completed |
| process | parameters | embossptsize | to be completed |
| process | parameters | asscript | to be completed |
| process | parameters | vectoroverlay | to be completed |
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

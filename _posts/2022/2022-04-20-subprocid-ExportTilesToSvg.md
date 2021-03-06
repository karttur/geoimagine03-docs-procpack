---
layout: subprocess
categories: subprocess
title: ExportTilesToSvg
processurl: subprocid-ExportTilesToSvg
rootprocid: Export
subprocid: ExportTilesToSvg
author: thomasg
excerpt: Export data to SVG
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
      "processid": "ExportTilesToSvg",
      "parameters": {
        "overwriteshade": "False",
        "overwritelayout": "False",
        "tolerance": "0",
        "simplify": "0",
        "scale": "0",
        "dstepsg": "4326",
        "stroke": "black",
        "fill": "none",
        "symbol": "None",
        "strokewidth": "1",
        "strokedasharray": "",
        "padding": "0",
        "pngsize": "",
        "crop": "",
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
        "hdr": "shp",
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
        "hdr": "svg",
        "dat": "png"
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
      "processid": "ExportTilesToSvg",
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
| process | parameters | overwriteshade | boolean | False | False |
| process | parameters | overwritelayout | boolean | False | False |
| process | parameters | tolerance | real | False | 0 |
| process | parameters | simplify | integer | False | 0 |
| process | parameters | scale | integer | False | 0 |
| process | parameters | dstepsg | integer | False | 4326 |
| process | parameters | stroke | text | False | black |
| process | parameters | fill | text | False | none |
| process | parameters | symbol | text | False | None |
| process | parameters | strokewidth | real | False | 1 |
| process | parameters | strokedasharray | text | False | --- |
| process | parameters | padding | integer | False | 0 |
| process | parameters | pngsize | text | False | --- |
| process | parameters | crop | text | False | --- |
| process | parameters | asscript | boolean | False | False |
| process | srccomp | * | element | True | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | shp |
| process | srcpath | dat | text | False | --- |
| process | dstcopy | layerid | text | False | copy |
| process | dstcopy | prefix | text | False | copy |
| process | dstcopy | srccomp | text | True | * |
| process | dstcopy | suffix | text | False | copy |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | svg |
| process | dstpath | dat | text | False | png |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | overwriteshade | to be completed |
| process | parameters | overwritelayout | to be completed |
| process | parameters | tolerance | to be completed |
| process | parameters | simplify | to be completed |
| process | parameters | scale | to be completed |
| process | parameters | dstepsg | to be completed |
| process | parameters | stroke | to be completed |
| process | parameters | fill | to be completed |
| process | parameters | symbol | to be completed |
| process | parameters | strokewidth | to be completed |
| process | parameters | strokedasharray | to be completed |
| process | parameters | padding | to be completed |
| process | parameters | pngsize | to be completed |
| process | parameters | crop | to be completed |
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

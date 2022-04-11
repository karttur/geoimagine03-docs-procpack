---
layout: subprocess
categories: subprocess
title: BasinOutletTiles
processurl: subprocid-BasinOutletTiles
rootprocid: BasinProc
subprocid: BasinOutletTiles
author: thomasg
excerpt: Refine pre-identified basin mouths in tiles data
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
      "processid": "BasinOutletTiles",
      "parameters": {
        "tiltmouths": "False",
        "grassdem": "DEM",
        "outlet": "MOUTH",
        "distill": "MOUTH",
        "clusteroutlet": "maximum",
        "basincelltrehshold": "-1",
        "watershed": "MFD",
        "memory": "300",
        "asscript": "True",
        "mosaic": "True"
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
      "dstcopy": {
        "layerid": "auto",
        "prefix": "auto",
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
      "processid": "BasinOutletTiles",
      "parameters": {
        "basincelltrehshold": "-1"
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
| process | parameters | tiltmouths | boolean | False | False |
| process | parameters | grassdem | text | False | DEM |
| process | parameters | outlet | text | False | MOUTH |
| process | parameters | distill | text | False | MOUTH |
| process | parameters | clusteroutlet | text | False | maximum |
| process | parameters | basincelltrehshold | integer | True | -1 |
| process | parameters | watershed | text | False | MFD |
| process | parameters | memory | integer | False | 300 |
| process | parameters | asscript | boolean | False | True |
| process | parameters | mosaic | boolean | False | True |
| process | srccomp | * | element | True | * |
| process | dstcopy | layerid | text | False | auto |
| process | dstcopy | prefix | text | False | auto |
| process | dstcopy | srccomp | text | True | * |
| process | dstcopy | suffix | text | False | auto |
| process | dstpath | volume | text | True | --- |

---
layout: subprocess
categories: subprocess
title: BasinOutletTiles
processurl: subprocid-BasinOutletTiles
rootprocid: BasinProc
subprocid: BasinOutletTiles
author: thomasg
excerpt: Refine pre-identified basin mouths in tiles data
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

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | tiltmouths | Tilt DEM at moouth to single outlet |
| process | parameters | grassdem | Name of GRASS internal DEM file (default: DEM) |
| process | parameters | outlet | MOUTH, SFD or MFD |
| process | parameters | distill | MFD, MOUTH or None |
| process | parameters | clusteroutlet | methods for finding single outlet point |
| process | parameters | basincelltrehshold | minimum nr of cells to form a basin |
| process | parameters | watershed | MFD [nr] or SFD |
| process | parameters | memory | memory assignment in MB |
| process | parameters | asscript | whether to run as script or inside python |
| process | parameters | mosaic | whether to use mosaicked tiles or not |
| process | srccomp | * | link for source composition |
| process | dstcopy | layerid | unknown hint |
| process | dstcopy | prefix | unknown hint |
| process | dstcopy | srccomp | unknown hint |
| process | dstcopy | suffix | unknown hint |
| process | dstpath | volume | to be completed |

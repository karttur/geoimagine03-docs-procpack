---
layout: subprocess
categories: subprocess
title: GrassDemFillDirTiles
processurl: subprocid-GrassDemFillDirTiles
rootprocid: GrassDemProc
subprocid: GrassDemFillDirTiles
author: thomasg
excerpt: Fill up dem pits
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
      "processid": "GrassDemFillDirTiles",
      "parameters": {
        "superimpose": "True",
        "singlewatershed": "True",
        "asscript": "True",
        "mosaic": "True",
        "memory": "4000",
        "pitsize": "4",
        "pitburnattribute": "filldem",
        "pitquery": "",
        "peaks": "False",
        "peakburnattribute": "nbdemq1",
        "peakquery": "",
        "tilesize": "2000",
        "tileoverlap": "10"
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
        "prefix": "*",
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
      "processid": "GrassDemFillDirTiles",
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
        "layerid": "*",
        "prefix": "*",
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
| process | parameters | superimpose | boolean | False | True |
| process | parameters | singlewatershed | boolean | False | True |
| process | parameters | asscript | boolean | False | True |
| process | parameters | mosaic | text | False | True |
| process | parameters | memory | integer | False | 4000 |
| process | parameters | pitsize | integer | False | 4 |
| process | parameters | pitburnattribute | text | False | filldem |
| process | parameters | pitquery | text | False | --- |
| process | parameters | peaks | boolean | False | False |
| process | parameters | peakburnattribute | text | False | nbdemq1 |
| process | parameters | peakquery | text | False | --- |
| process | parameters | tilesize | integer | False | 2000 |
| process | parameters | tileoverlap | integer | False | 10 |
| process | srccomp | * | element | True | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcopy | layerid | text | True | * |
| process | dstcopy | prefix | text | True | * |
| process | dstcopy | srccomp | text | True | * |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | superimpose | to be completed |
| process | parameters | singlewatershed | to be completed |
| process | parameters | asscript | to be completed |
| process | parameters | mosaic | to be completed |
| process | parameters | memory | to be completed |
| process | parameters | pitsize | Only remove sinks not larger than <pitsize> cells |
| process | parameters | pitburnattribute | Attribute to use for burning DEM |
| process | parameters | pitquery | Query for filling pits |
| process | parameters | peaks | Remove single peaks or not. |
| process | parameters | peakburnattribute | Attribute to use for burning DEM |
| process | parameters | peakquery | Query for flattening peaks |
| process | parameters | tilesize | Tile size (pixels) for dividing DEM raster |
| process | parameters | tileoverlap | Tile overlap for dividing DEM raster  |
| process | srccomp | * | link for source composition |
| process | srcpath | volume | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | dat | to be completed |
| process | dstcopy | layerid | unknown hint |
| process | dstcopy | prefix | unknown hint |
| process | dstcopy | srccomp | unknown hint |
| process | dstpath | volume | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | dat | to be completed |

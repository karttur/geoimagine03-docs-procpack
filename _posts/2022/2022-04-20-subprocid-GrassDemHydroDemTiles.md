---
layout: subprocess
categories: subprocess
title: GrassDemHydroDemTiles
processurl: subprocid-GrassDemHydroDemTiles
rootprocid: GrassDemProc
subprocid: GrassDemHydroDemTiles
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
      "processid": "GrassDemHydroDemTiles",
      "parameters": {
        "superimpose": "True",
        "asscript": "True",
        "mosaic": "True",
        "flags": "",
        "size": "4",
        "mod": "4",
        "diffthreshold": "0.01",
        "query": "",
        "memory": "300",
        "tilesize": "1000",
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
      "processid": "GrassDemHydroDemTiles",
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
| process | parameters | asscript | boolean | False | True |
| process | parameters | mosaic | text | False | True |
| process | parameters | flags | text | False | --- |
| process | parameters | size | integer | False | 4 |
| process | parameters | mod | integer | False | 4 |
| process | parameters | diffthreshold | float | False | 0.01 |
| process | parameters | query | text | False | --- |
| process | parameters | memory | integer | False | 300 |
| process | parameters | tilesize | integer | False | 1000 |
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
| process | parameters | asscript | to be completed |
| process | parameters | mosaic | to be completed |
| process | parameters | flags | to be completed |
| process | parameters | size | Only remove sinks not larger than <size> cells |
| process | parameters | mod |  |
| process | parameters | diffthreshold | min difference original DEM and HydroDEM to count as change |
| process | parameters | query | Query for burning hydrodem corrections |
| process | parameters | memory | Memory allocation |
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

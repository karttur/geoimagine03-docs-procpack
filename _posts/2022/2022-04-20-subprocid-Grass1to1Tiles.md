---
layout: subprocess
categories: subprocess
title: Grass1to1Tiles
processurl: subprocid-Grass1to1Tiles
rootprocid: GrassProc
subprocid: Grass1to1Tiles
author: thomasg
excerpt: Grass binding for tile processes 1 to 1
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
      "processid": "Grass1to1Tiles",
      "parameters": {
        "mosaic": "False",
        "asscript": "False",
        "regionlayer": "",
        "subparameter": [
          {
            "grass.command": {
              "parameter1": "value1",
              "parameter..n": "value..n"
            }
          },
          {
            "grass.command": {
              "parameter1": "value1",
              "parameter..n": "value..n"
            }
          }
        ]
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
        "cellnull": "auto",
        "celltype": "auto",
        "content": "",
        "dataunit": "auto",
        "layerid": "*",
        "masked": "N",
        "measure": "auto",
        "offsetadd": "0",
        "prefix": "",
        "product": "",
        "scalefac": "1",
        "source": "",
        "srccomp": "*",
        "suffix": ""
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
      "processid": "Grass1to1Tiles",
      "parameters": {
        "regionlayer": "",
        "subparameter": [
          {
            "grass.command": {
              "parameter1": "value1",
              "parameter..n": "value..n"
            }
          },
          {
            "grass.command": {
              "parameter1": "value1",
              "parameter..n": "value..n"
            }
          }
        ]
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
        "content": "",
        "layerid": "*",
        "prefix": "",
        "product": "",
        "source": "",
        "srccomp": "*",
        "suffix": ""
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
| process | parameters | mosaic | boolean | False | False |
| process | parameters | asscript | boolean | False | False |
| process | parameters | regionlayer | text | True | --- |
| process | parameters | subparameter | list | True | --- |
| process | srccomp | * | element | True | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcopy | cellnull | text | False | auto |
| process | dstcopy | celltype | text | False | auto |
| process | dstcopy | content | text | True | --- |
| process | dstcopy | dataunit | text | False | auto |
| process | dstcopy | layerid | text | True | * |
| process | dstcopy | masked | text | False | N |
| process | dstcopy | measure | text | False | auto |
| process | dstcopy | offsetadd | integer | False | 0 |
| process | dstcopy | prefix | text | True | --- |
| process | dstcopy | product | text | True | --- |
| process | dstcopy | scalefac | real | False | 1 |
| process | dstcopy | source | text | True | --- |
| process | dstcopy | srccomp | text | True | * |
| process | dstcopy | suffix | text | True | --- |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | mosaic | to be completed |
| process | parameters | asscript | to be completed |
| process | parameters | regionlayer | Layer that defined the default region of the location |
| process | parameters | subparameter | to be completed |
| process | srccomp | * | link for source composition |
| process | srcpath | volume | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | dat | to be completed |
| process | dstcopy | cellnull | unknown hint |
| process | dstcopy | celltype | unknown hint |
| process | dstcopy | content | Import layer content or theme (hyphen allowed, underscore not allowd) |
| process | dstcopy | dataunit | unknown hint |
| process | dstcopy | layerid | Import layer id |
| process | dstcopy | masked | Whether the data is masked or not |
| process | dstcopy | measure | unknown hint |
| process | dstcopy | offsetadd | Offset add default = 0, no adding |
| process | dstcopy | prefix | Import layer prefix (usually identical to layerid) |
| process | dstcopy | product | Import layer product, producer or similary (hyphen allowed, underscore not allowd) |
| process | dstcopy | scalefac | Scale factor for raster data (default = 1.0, no scaling) |
| process | dstcopy | source | Source instrument, method, model or similar of import layer (hyphen allowed, underscore not allowd) |
| process | dstcopy | srccomp | unknown hint |
| process | dstcopy | suffix | Import layer syffix (usually identical to id) |
| process | dstpath | volume | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | dat | to be completed |

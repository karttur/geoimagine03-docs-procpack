---
layout: subprocess
categories: subprocess
title: UpdateDbTiles
processurl: subprocid-UpdateDbTiles
rootprocid: UpdateDb
subprocid: UpdateDbTiles
author: thomasg
excerpt: Update
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
      "processid": "UpdateDbTiles",
      "parameters": {
        "dummy": "dummy"
      },
      "dstcomp": [
        {
          "user_def_1": {
            "cellnull": "",
            "celltype": "",
            "content": "",
            "dataunit": "",
            "layerid": "*",
            "masked": "N",
            "measure": "N",
            "offsetadd": "0",
            "prefix": "",
            "product": "",
            "scalefac": "1",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "cellnull": "",
            "celltype": "",
            "content": "",
            "dataunit": "",
            "layerid": "*",
            "masked": "N",
            "measure": "N",
            "offsetadd": "0",
            "prefix": "",
            "product": "",
            "scalefac": "1",
            "source": "",
            "suffix": ""
          }
        }
      ],
      "dstpath": {
        "volume": "",
        "hdr": "shp",
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
      "processid": "UpdateDbTiles",
      "parameters": {},
      "dstcomp": [
        {
          "user_def_1": {
            "cellnull": "",
            "celltype": "",
            "content": "",
            "dataunit": "",
            "layerid": "*",
            "masked": "N",
            "measure": "N",
            "offsetadd": "0",
            "prefix": "",
            "product": "",
            "scalefac": "1",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "cellnull": "",
            "celltype": "",
            "content": "",
            "dataunit": "",
            "layerid": "*",
            "masked": "N",
            "measure": "N",
            "offsetadd": "0",
            "prefix": "",
            "product": "",
            "scalefac": "1",
            "source": "",
            "suffix": ""
          }
        }
      ],
      "dstpath": {
        "volume": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | dummy | text | False | dummy |
| process | dstcomp | element | text | False | * |
| process | dstcomp | layer | element | True | * |
| process | dstcomp | parent | text | False | process |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | shp |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | dummy | to be completed |
| process | dstcomp | element | to be completed |
| process | dstcomp | layer | to be completed |
| process | dstcomp | parent | to be completed |
| process | dstpath | volume | Volume, disk or path for saving the destination data |
| process | dstpath | hdr | Header or header+data file extension (default = shp) |
| process | dstpath | dat | Data file extension for datasets with separate header + data file |

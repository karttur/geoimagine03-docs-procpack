---
layout: subprocess
categories: subprocess
title: TractFromVector
processurl: subprocid-TractFromVector
rootprocid: ManageRegion
subprocid: TractFromVector
author: thomasg
excerpt: Define tract from extent
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
      "processid": "TractFromVector",
      "parameters": {
        "defaultregion": "",
        "tractid": "",
        "tracttitle": "",
        "tractlabel": "",
        "buffer": "0"
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
        "dat": "",
        "hdr": "shp",
        "volume": ""
      },
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
      "processid": "TractFromVector",
      "parameters": {
        "defaultregion": "",
        "tractid": "",
        "tracttitle": ""
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
        "volume": ""
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
| process | parameters | defaultregion | text | True | --- |
| process | parameters | tractid | text | True | --- |
| process | parameters | tracttitle | text | True | --- |
| process | parameters | tractlabel | text | False | --- |
| process | parameters | buffer | float | False | 0 |
| process | srccomp | element | text | False | process |
| process | srccomp | parent | text | False | process |
| process | srccomp | srctractextent | element | True | --- |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | False | shp |
| process | srcpath | volume | text | True | --- |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | shp |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | defaultregion | Select a default region to use for defining your tract |
| process | parameters | tractid | Set a unique tractid |
| process | parameters | tracttitle | Give a title for the new tract (for maps) |
| process | parameters | tractlabel | Give a label for the tract |
| process | parameters | buffer | Buffer in map units to expand region comapred to data points |
| process | srccomp | element | Default hierarchical child name |
| process | srccomp | parent | Hierarchical object parent (for internal use) |
| process | srccomp | srctractextent | Hierarchical pointer |
| process | srcpath | dat | Data file extension for datasets with separate header + data file |
| process | srcpath | hdr | Header or header+data file extension (default = shp) |
| process | srcpath | volume | Volume, disk or path containg the source data |
| process | dstpath | volume | Volume, disk or path for saving the destination data |
| process | dstpath | hdr | Header or header+data file extension (default = shp) |
| process | dstpath | dat | Data file extension for datasets with separate header + data file |

---
layout: subprocess
categories: subprocess
title: SiteFromVector
processurl: subprocid-SiteFromVector
rootprocid: ManageRegion
subprocid: SiteFromVector
author: thomasg
excerpt: Define site from extent
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
      "processid": "SiteFromVector",
      "parameters": {
        "tractid": "",
        "siteid": "",
        "sitetitle": "",
        "sitelabel": "",
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
      "processid": "SiteFromVector",
      "parameters": {
        "tractid": "",
        "siteid": "",
        "sitetitle": ""
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
| process | parameters | tractid | text | True | --- |
| process | parameters | siteid | text | True | --- |
| process | parameters | sitetitle | text | True | --- |
| process | parameters | sitelabel | text | False | --- |
| process | parameters | buffer | float | False | 0 |
| process | srccomp | element | text | False | process |
| process | srccomp | parent | text | False | process |
| process | srccomp | srcsiteextent | element | True | --- |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | False | shp |
| process | srcpath | volume | text | True | --- |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | shp |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | tractid | Select a tract to use for defining your site |
| process | parameters | siteid | Set a unique siteid |
| process | parameters | sitetitle | Give a title for the new site (for maps) |
| process | parameters | sitelabel | Give a label for the site |
| process | parameters | buffer | Buffer in map units to expand site comapred to data points |
| process | srccomp | element | Default hierarchical child name |
| process | srccomp | parent | Hierarchical object parent (for internal use) |
| process | srccomp | srcsiteextent | Hierarchical pointer |
| process | srcpath | dat | Data file extension for datasets with separate header + data file |
| process | srcpath | hdr | Header or header+data file extension (default = shp) |
| process | srcpath | volume | Volume, disk or path containg the source data |
| process | dstpath | volume | Volume, disk or path for saving the destination data |
| process | dstpath | hdr | Header or header+data file extension (default = shp) |
| process | dstpath | dat | Data file extension for datasets with separate header + data file |

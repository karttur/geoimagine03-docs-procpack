---
layout: subprocess
categories: subprocess
title: OrganizeGrace
processurl: subprocid-OrganizeGrace
rootprocid: GraceProc
subprocid: OrganizeGrace
author: thomasg
excerpt: Organize grace data
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
      "processid": "OrganizeGrace",
      "parameters": {
        "feature": "land_mass",
        "model": "RL06",
        "version": "v03",
        "solutionset": "JPL",
        "accessdate": "",
        "dataurl": "",
        "metaurl": "",
        "title": "",
        "label": "",
        "replacestr": "",
        "replacetag": "",
        "cellnull": "-99999.0"
      },
      "srcpath": {
        "dat": "",
        "hdr": "",
        "volume": ""
      },
      "dstpath": {
        "dat": "",
        "hdr": "tif",
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
      "processid": "OrganizeGrace",
      "parameters": {
        "dataurl": "",
        "metaurl": ""
      },
      "srcpath": {
        "hdr": "",
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
| process | parameters | feature | text | False | land_mass |
| process | parameters | model | text | False | RL06 |
| process | parameters | version | text | False | v03 |
| process | parameters | solutionset | text | False | JPL |
| process | parameters | accessdate | text | False | --- |
| process | parameters | dataurl | text | True | --- |
| process | parameters | metaurl | text | True | --- |
| process | parameters | title | text | False | --- |
| process | parameters | label | text | False | --- |
| process | parameters | replacestr | text | False | --- |
| process | parameters | replacetag | text | False | --- |
| process | parameters | cellnull | float | False | -99999.0 |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | True | --- |
| process | srcpath | volume | text | True | --- |
| process | dstpath | dat | text | False | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | feature | to be completed |
| process | parameters | model | to be completed |
| process | parameters | version | to be completed |
| process | parameters | solutionset | to be completed |
| process | parameters | accessdate | Date of accessing dataset (if left blank todays date will be recorded) |
| process | parameters | dataurl | url for source dataset |
| process | parameters | metaurl | url for source metadata |
| process | parameters | title | Source dataset title |
| process | parameters | label | Source dataset label |
| process | parameters | replacestr | String to replace in multi-layered source datasets |
| process | parameters | replacetag | Tag identifying replacement identifying |
| process | parameters | cellnull | cellnull for GRACE data to organize |
| process | srcpath | dat | Data file extension for datasets with separate header + data file |
| process | srcpath | hdr | Header or header+data file extension |
| process | srcpath | volume | Volume, disk or path containg the source data |
| process | dstpath | dat | Data file extension for datasets with separate header + data file |
| process | dstpath | hdr | Header or header+data file extension (default = shp) |
| process | dstpath | volume | Volume, disk or path for saving the destination data |

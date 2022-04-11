---
layout: subprocess
categories: subprocess
title: OrganizeGrace
processurl: subprocid-OrganizeGrace
rootprocid: GraceProc
subprocid: OrganizeGrace
author: thomasg
excerpt: Organize grace data
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

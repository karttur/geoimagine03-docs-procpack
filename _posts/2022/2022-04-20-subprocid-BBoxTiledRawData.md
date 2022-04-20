---
layout: subprocess
categories: subprocess
title: BBoxTiledRawData
processurl: subprocid-BBoxTiledRawData
rootprocid: Ancillary
subprocid: BBoxTiledRawData
author: thomasg
excerpt: Bounding box for raw tiles
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
      "processid": "BBoxTiledRawData",
      "parameters": {
        "getlist": "csvfile-getpath1",
        "srcdir": "",
        "dstdir": "",
        "pattern": "",
        "nonpattern": ""
      },
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
      "processid": "BBoxTiledRawData",
      "parameters": {
        "getlist": "csvfile-getpath1",
        "srcdir": "",
        "dstdir": ""
      },
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
| process | parameters | getlist | text | True | csvfile-getpath1 |
| process | parameters | srcdir | text | True | --- |
| process | parameters | dstdir | text | True | --- |
| process | parameters | pattern | csvlist | False | --- |
| process | parameters | nonpattern | csvlist | False | --- |
| process | srcpath | volume | text | True | --- |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | getlist | Alternatives for getting the files to unzip |
| process | parameters | srcdir | Path to folder holding raw data tiles |
| process | parameters | dstdir | Path to vector file |
| process | parameters | pattern | list csv search terms for identifying valid tiles |
| process | parameters | nonpattern | list csv search terms for excluding non-valid tiles |
| process | srcpath | volume | to be completed |
| process | dstpath | volume | to be completed |

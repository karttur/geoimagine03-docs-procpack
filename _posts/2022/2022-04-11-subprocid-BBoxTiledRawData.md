---
layout: subprocess
categories: subprocess
title: BBoxTiledRawData
processurl: subprocid-BBoxTiledRawData
rootprocid: Ancillary
subprocid: BBoxTiledRawData
author: thomasg
excerpt: Bounding box for raw tiles
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

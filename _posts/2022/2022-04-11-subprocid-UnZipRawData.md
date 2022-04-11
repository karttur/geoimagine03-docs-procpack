---
layout: subprocess
categories: subprocess
title: UnZipRawData
processurl: subprocid-UnZipRawData
rootprocid: Ancillary
subprocid: UnZipRawData
author: thomasg
excerpt: Search local geojson file for tiles to unzip
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
      "processid": "UnZipRawData",
      "parameters": {
        "getlist": "csvfile-getpath1",
        "pattern": "",
        "patternreplace": "pattern",
        "zipreplace": ".tif",
        "srcdir": "",
        "dstdir": "",
        "minlon": "-180",
        "minlat": "-90",
        "maxlon": "180",
        "maxlat": "90"
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
      "processid": "UnZipRawData",
      "parameters": {
        "getlist": "csvfile-getpath1",
        "pattern": "",
        "zipreplace": ".tif",
        "srcdir": "",
        "dstdir": ""
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
| process | parameters | pattern | text | True | --- |
| process | parameters | patternreplace | text | False | pattern |
| process | parameters | zipreplace | text | True | .tif |
| process | parameters | srcdir | text | True | --- |
| process | parameters | dstdir | text | True | --- |
| process | parameters | minlon | integer | False | -180 |
| process | parameters | minlat | integer | False | -90 |
| process | parameters | maxlon | integer | False | 180 |
| process | parameters | maxlat | integer | False | 90 |
| process | dstpath | volume | text | True | --- |

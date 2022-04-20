---
layout: subprocess
categories: subprocess
title: UnZipRawData
processurl: subprocid-UnZipRawData
rootprocid: Ancillary
subprocid: UnZipRawData
author: thomasg
excerpt: Search local geojson file for tiles to unzip
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

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | getlist | Alternatives for getting the files to unzip |
| process | parameters | pattern | pattern to search in zip file |
| process | parameters | patternreplace | Replace string for search pattern |
| process | parameters | zipreplace | extention replace string |
| process | parameters | srcdir | Path to json object listing urls |
| process | parameters | dstdir | Subdir with zip files |
| process | parameters | minlon | Minimum longitude |
| process | parameters | minlat | Minimum latitude |
| process | parameters | maxlon | Maximum longitude |
| process | parameters | maxlat | Maximum latitude |
| process | dstpath | volume | to be completed |

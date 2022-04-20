---
layout: subprocess
categories: subprocess
title: UnZipTandemX
processurl: subprocid-UnZipTandemX
rootprocid: Ancillary
subprocid: UnZipTandemX
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
      "processid": "UnZipTandemX",
      "parameters": {
        "path": "",
        "datadir": "",
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
      "processid": "UnZipTandemX",
      "parameters": {
        "path": "",
        "datadir": ""
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
| process | parameters | path | text | True | --- |
| process | parameters | datadir | text | True | --- |
| process | parameters | minlon | integer | False | -180 |
| process | parameters | minlat | integer | False | -90 |
| process | parameters | maxlon | integer | False | 180 |
| process | parameters | maxlat | integer | False | 90 |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | path | Path to json object listing urls |
| process | parameters | datadir | Dst datadir for downloads |
| process | parameters | minlon | Minimum longitude |
| process | parameters | minlat | Minimum latitude |
| process | parameters | maxlon | Maximum longitude |
| process | parameters | maxlat | Maximum latitude |
| process | dstpath | volume | to be completed |

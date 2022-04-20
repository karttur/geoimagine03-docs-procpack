---
layout: subprocess
categories: subprocess
title: GeoCheckSentinelTiles
processurl: subprocid-GeoCheckSentinelTiles
rootprocid: SentinelProcess
subprocid: GeoCheckSentinelTiles
author: thomasg
excerpt: Check geolocation of sentinel tile
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
      "processid": "GeoCheckSentinelTiles",
      "parameters": {
        "orbitdirection": "B",
        "platformname": "Sentinel-2",
        "prodtype": "S2MSI1C"
      },
      "srcpath": {
        "dat": "tif",
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
      "processid": "GeoCheckSentinelTiles",
      "parameters": {
        "orbitdirection": "B",
        "platformname": "Sentinel-2",
        "prodtype": "S2MSI1C"
      },
      "srcpath": {
        "volume": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | orbitdirection | text | True | B |
| process | parameters | platformname | text | True | Sentinel-2 |
| process | parameters | prodtype | text | True | S2MSI1C |
| process | srcpath | dat | text | False | tif |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | orbitdirection | to be completed |
| process | parameters | platformname | to be completed |
| process | parameters | prodtype | to be completed |
| process | srcpath | dat | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | volume | to be completed |

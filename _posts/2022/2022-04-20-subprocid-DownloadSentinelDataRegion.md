---
layout: subprocess
categories: subprocess
title: DownloadSentinelDataRegion
processurl: subprocid-DownloadSentinelDataRegion
rootprocid: SentinelProcess
subprocid: DownloadSentinelDataRegion
author: thomasg
excerpt: Download Sentinel data
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
      "processid": "DownloadSentinelDataRegion",
      "parameters": {
        "tiles": "True",
        "orbitdirection": "B",
        "platformname": "Sentinel-2",
        "downloaded": "N",
        "prodtype": "S2MSI1C",
        "cloudmax": "30"
      },
      "srcpath": {
        "dat": "shp",
        "hdr": "shp",
        "volume": ""
      },
      "dstpath": {
        "dat": "zip",
        "hdr": "zip",
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
      "processid": "DownloadSentinelDataRegion",
      "parameters": {
        "orbitdirection": "B",
        "platformname": "Sentinel-2",
        "prodtype": "S2MSI1C"
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
| process | parameters | tiles | bool | False | True |
| process | parameters | orbitdirection | text | True | B |
| process | parameters | platformname | text | True | Sentinel-2 |
| process | parameters | downloaded | text | False | N |
| process | parameters | prodtype | text | True | S2MSI1C |
| process | parameters | cloudmax | integer | False | 30 |
| process | srcpath | dat | text | False | shp |
| process | srcpath | hdr | text | False | shp |
| process | srcpath | volume | text | True | --- |
| process | dstpath | dat | text | False | zip |
| process | dstpath | hdr | text | False | zip |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | tiles | to be completed |
| process | parameters | orbitdirection | to be completed |
| process | parameters | platformname | to be completed |
| process | parameters | downloaded | to be completed |
| process | parameters | prodtype | to be completed |
| process | parameters | cloudmax | to be completed |
| process | srcpath | dat | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | volume | to be completed |
| process | dstpath | dat | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | volume | to be completed |

---
layout: subprocess
categories: subprocess
title: DownloadSentinelTile
processurl: subprocid-DownloadSentinelTile
rootprocid: SentinelProcess
subprocid: DownloadSentinelTile
author: thomasg
excerpt: Download Sentinel data
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
      "processid": "DownloadSentinelTile",
      "parameters": {
        "tileid": "tileid",
        "orbitdirection": "B",
        "platformname": "Sentinel-2",
        "downloaded": "N",
        "prodtype": "S2MSI1C",
        "cloudmax": "30"
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
      "processid": "DownloadSentinelTile",
      "parameters": {
        "tileid": "tileid"
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
| process | parameters | tileid | string | True | tileid |
| process | parameters | orbitdirection | text | False | B |
| process | parameters | platformname | text | False | Sentinel-2 |
| process | parameters | downloaded | text | False | N |
| process | parameters | prodtype | text | False | S2MSI1C |
| process | parameters | cloudmax | integer | False | 30 |
| process | dstpath | dat | text | False | zip |
| process | dstpath | hdr | text | False | zip |
| process | dstpath | volume | text | True | --- |

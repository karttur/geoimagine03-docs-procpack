---
layout: subprocess
categories: subprocess
title: DownloadSentinelData
processurl: subprocid-DownloadSentinelData
rootprocid: SentinelProcess
subprocid: DownloadSentinelData
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
      "processid": "DownloadSentinelData",
      "parameters": {
        "tiles": "True",
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
      "processid": "DownloadSentinelData",
      "parameters": {
        "orbitdirection": "B",
        "platformname": "Sentinel-2",
        "prodtype": "S2MSI1C"
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
| process | dstpath | dat | text | False | zip |
| process | dstpath | hdr | text | False | zip |
| process | dstpath | volume | text | True | --- |

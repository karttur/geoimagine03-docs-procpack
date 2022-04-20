---
layout: subprocess
categories: subprocess
title: ReorganiseSentinel
processurl: subprocid-ReorganiseSentinel
rootprocid: SentinelProcess
subprocid: ReorganiseSentinel
author: thomasg
excerpt: Reorganize Sentinel tiles and granules
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
      "processid": "ReorganiseSentinel",
      "parameters": {
        "searchpath": "",
        "tiles": "True",
        "platformname": "Sentinel-2",
        "prodtype": "S2MSI1C"
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
      "processid": "ReorganiseSentinel",
      "parameters": {
        "searchpath": "",
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
| process | parameters | searchpath | string | True | --- |
| process | parameters | tiles | bool | False | True |
| process | parameters | platformname | text | True | Sentinel-2 |
| process | parameters | prodtype | text | True | S2MSI1C |
| process | dstpath | dat | text | False | zip |
| process | dstpath | hdr | text | False | zip |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | searchpath | to be completed |
| process | parameters | tiles | to be completed |
| process | parameters | platformname | to be completed |
| process | parameters | prodtype | to be completed |
| process | dstpath | dat | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | volume | to be completed |

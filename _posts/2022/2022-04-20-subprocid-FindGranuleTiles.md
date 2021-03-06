---
layout: subprocess
categories: subprocess
title: FindGranuleTiles
processurl: subprocid-FindGranuleTiles
rootprocid: SentinelProcess
subprocid: FindGranuleTiles
author: thomasg
excerpt: Find mgrs tiles covered by granulue
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
      "processid": "FindGranuleTiles",
      "parameters": {
        "granuleoverlap": "0.1",
        "platformname": "Sentinel-2",
        "downloaded": "N",
        "prodtype": "GRD",
        "mgrsversion": "NGA",
        "cloudmax": "100"
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
      "processid": "FindGranuleTiles",
      "parameters": {},
      "dstpath": {
        "volume": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | granuleoverlap | float | False | 0.1 |
| process | parameters | platformname | text | False | Sentinel-2 |
| process | parameters | downloaded | text | False | N |
| process | parameters | prodtype | text | False | GRD |
| process | parameters | mgrsversion | text | False | NGA |
| process | parameters | cloudmax | integer | False | 100 |
| process | dstpath | dat | text | False | zip |
| process | dstpath | hdr | text | False | zip |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | granuleoverlap | to be completed |
| process | parameters | platformname | to be completed |
| process | parameters | downloaded | to be completed |
| process | parameters | prodtype | to be completed |
| process | parameters | mgrsversion | to be completed |
| process | parameters | cloudmax | to be completed |
| process | dstpath | dat | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | volume | to be completed |

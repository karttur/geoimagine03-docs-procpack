---
layout: subprocess
categories: subprocess
title: CurlGrace
processurl: subprocid-CurlGrace
rootprocid: GraceProc
subprocid: CurlGrace
author: thomasg
excerpt: Curl Grace data via html coded url
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
      "processid": "CurlGrace",
      "parameters": {
        "feature": "land_mass",
        "content": "RL06",
        "version": "v03",
        "source": "JPL",
        "remoteuser": "",
        "serverurl": ""
      },
      "srcpath": {
        "hdr": "tif",
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
      "processid": "CurlGrace",
      "parameters": {
        "remoteuser": "",
        "serverurl": ""
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
| process | parameters | feature | text | False | land_mass |
| process | parameters | content | text | False | RL06 |
| process | parameters | version | text | False | v03 |
| process | parameters | source | text | False | JPL |
| process | parameters | remoteuser | text | True | --- |
| process | parameters | serverurl | text | True | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | volume | text | True | --- |
| process | dstpath | volume | text | True | --- |

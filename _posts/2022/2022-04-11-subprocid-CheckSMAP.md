---
layout: subprocess
categories: subprocess
title: CheckSMAP
processurl: subprocid-CheckSMAP
rootprocid: SmapProc
subprocid: CheckSMAP
author: thomasg
excerpt: Check SMAP download and extraction>
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
      "processid": "CheckSMAP",
      "parameters": {
        "product": "",
        "version": ""
      },
      "srcpath": {
        "dat": "",
        "hdr": "h5",
        "volume": ""
      },
      "dstpath": {
        "dat": "",
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
      "processid": "CheckSMAP",
      "parameters": {
        "product": "",
        "version": ""
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
| process | parameters | product | text | True | --- |
| process | parameters | version | text | True | --- |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | False | h5 |
| process | srcpath | volume | text | True | --- |
| process | dstpath | dat | text | False | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | volume | text | True | --- |

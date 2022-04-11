---
layout: subprocess
categories: subprocess
title: DownloadUSGS
processurl: subprocid-DownloadUSGS
rootprocid: USGSProc
subprocid: DownloadUSGS
author: thomasg
excerpt: Download USGS data
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
      "processid": "DownloadUSGS",
      "parameters": {
        "remoteuser": "user",
        "password": "password",
        "searchdone": "False",
        "product": "MCD43A4",
        "version": "006"
      },
      "dstpath": {
        "dat": "hdf",
        "hdr": "hdf",
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
      "processid": "DownloadUSGS",
      "parameters": {
        "product": "MCD43A4",
        "version": "006"
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
| process | parameters | remoteuser | text | False | user |
| process | parameters | password | text | False | password |
| process | parameters | searchdone | text | False | False |
| process | parameters | product | text | True | MCD43A4 |
| process | parameters | version | text | True | 006 |
| process | dstpath | dat | text | False | hdf |
| process | dstpath | hdr | text | False | hdf |
| process | dstpath | volume | text | True | --- |

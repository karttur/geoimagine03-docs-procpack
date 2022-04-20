---
layout: subprocess
categories: subprocess
title: DownLoadModisPolar
processurl: subprocid-DownLoadModisPolar
rootprocid: ModisPolar
subprocid: DownLoadModisPolar
author: thomasg
excerpt: Download MODIS data from NSIDC
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
      "processid": "DownLoadModisPolar",
      "parameters": {
        "searchdone": "false",
        "remoteuser": "",
        "asscript": "True",
        "serverurl": "https://n5eil01u.ecs.nsidc.org",
        "downloaded": "N",
        "product": "MYD10A2",
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
      "processid": "DownLoadModisPolar",
      "parameters": {
        "remoteuser": "",
        "product": "MYD10A2",
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
| process | parameters | searchdone | bool | False | false |
| process | parameters | remoteuser | text | True | --- |
| process | parameters | asscript | boolean | False | True |
| process | parameters | serverurl | text | False | https://n5eil01u.ecs.nsidc.org |
| process | parameters | downloaded | text | False | N |
| process | parameters | product | text | True | MYD10A2 |
| process | parameters | version | text | True | 006 |
| process | dstpath | dat | text | False | hdf |
| process | dstpath | hdr | text | False | hdf |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | searchdone | to be completed |
| process | parameters | remoteuser | to be completed |
| process | parameters | asscript | to be completed |
| process | parameters | serverurl | to be completed |
| process | parameters | downloaded | to be completed |
| process | parameters | product | to be completed |
| process | parameters | version | to be completed |
| process | dstpath | dat | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | volume | to be completed |

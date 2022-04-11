---
layout: subprocess
categories: subprocess
title: DownLoadModisPolar
processurl: subprocid-DownLoadModisPolar
rootprocid: ModisPolar
subprocid: DownLoadModisPolar
author: thomasg
excerpt: Download MODIS data from NSIDC
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

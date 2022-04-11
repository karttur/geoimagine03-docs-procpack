---
layout: subprocess
categories: subprocess
title: DownLoadSmapDaac
processurl: subprocid-DownLoadSmapDaac
rootprocid: SmapProc
subprocid: DownLoadSmapDaac
author: thomasg
excerpt: Download SMAP data from DAAC
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
      "processid": "DownLoadSmapDaac",
      "parameters": {
        "remoteuser": "",
        "asscript": "True",
        "serverurl": "https://n5eil01u.ecs.nsidc.org",
        "searchdone": "False",
        "product": "SPL3SMP_E",
        "version": "002"
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
      "processid": "DownLoadSmapDaac",
      "parameters": {
        "remoteuser": "",
        "product": "SPL3SMP_E",
        "version": "002"
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
| process | parameters | remoteuser | text | True | --- |
| process | parameters | asscript | boolean | False | True |
| process | parameters | serverurl | text | False | https://n5eil01u.ecs.nsidc.org |
| process | parameters | searchdone | Boolean | False | False |
| process | parameters | product | text | True | SPL3SMP_E |
| process | parameters | version | text | True | 002 |
| process | dstpath | dat | text | False | hdf |
| process | dstpath | hdr | text | False | hdf |
| process | dstpath | volume | text | True | --- |

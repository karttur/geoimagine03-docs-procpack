---
layout: subprocess
categories: subprocess
title: ExtractSmapHdf
processurl: subprocid-ExtractSmapHdf
rootprocid: SmapProc
subprocid: ExtractSmapHdf
author: thomasg
excerpt: Extracts the content of SMAP HDF>
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
      "processid": "ExtractSmapHdf",
      "parameters": {
        "asscript": "True",
        "product": "MYD29E1D",
        "version": "006",
        "remoteuser": "",
        "serverurl": "https://n5eil01u.ecs.nsidc.org",
        "searchdone": "True"
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
      "processid": "ExtractSmapHdf",
      "parameters": {
        "product": "MYD29E1D",
        "version": "006",
        "remoteuser": "",
        "serverurl": "https://n5eil01u.ecs.nsidc.org"
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
| process | parameters | asscript | boolean | False | True |
| process | parameters | product | text | True | MYD29E1D |
| process | parameters | version | text | True | 006 |
| process | parameters | remoteuser | text | True | --- |
| process | parameters | serverurl | text | True | https://n5eil01u.ecs.nsidc.org |
| process | parameters | searchdone | Boolean | False | True |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | False | h5 |
| process | srcpath | volume | text | True | --- |
| process | dstpath | dat | text | False | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | volume | text | True | --- |

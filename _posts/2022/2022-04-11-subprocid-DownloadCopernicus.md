---
layout: subprocess
categories: subprocess
title: DownloadCopernicus
processurl: subprocid-DownloadCopernicus
rootprocid: CopernicusProc
subprocid: DownloadCopernicus
author: thomasg
excerpt: Download Copernicus data
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
      "processid": "DownloadCopernicus",
      "parameters": {
        "serverurl": "gisco-services.ec.europa.eu",
        "remoteuser": "user",
        "password": "password",
        "searchdone": "False",
        "product": "",
        "version": ""
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
      "processid": "DownloadCopernicus",
      "parameters": {
        "product": "",
        "version": ""
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
| process | parameters | serverurl | text | False | gisco-services.ec.europa.eu |
| process | parameters | remoteuser | text | False | user |
| process | parameters | password | text | False | password |
| process | parameters | searchdone | text | False | False |
| process | parameters | product | text | True | --- |
| process | parameters | version | text | True | --- |
| process | dstpath | dat | text | False | hdf |
| process | dstpath | hdr | text | False | hdf |
| process | dstpath | volume | text | True | --- |

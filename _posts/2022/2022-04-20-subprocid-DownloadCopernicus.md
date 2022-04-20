---
layout: subprocess
categories: subprocess
title: DownloadCopernicus
processurl: subprocid-DownloadCopernicus
rootprocid: CopernicusProc
subprocid: DownloadCopernicus
author: thomasg
excerpt: Download Copernicus data
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
      "processid": "DownloadCopernicus",
      "parameters": {
        "serverurl": "gisco-services.ec.europa.eu",
        "remoteuser": "user",
        "password": "password",
        "searchdone": "False",
        "localhtml": "copdem.html",
        "regex": "*",
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
| process | parameters | localhtml | text | False | copdem.html |
| process | parameters | regex | text | False | * |
| process | parameters | product | text | True | --- |
| process | parameters | version | text | True | --- |
| process | dstpath | dat | text | False | hdf |
| process | dstpath | hdr | text | False | hdf |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | serverurl | Serverurl for Copernicus data |
| process | parameters | remoteuser | Server user |
| process | parameters | password | Server password |
| process | parameters | searchdone | Re-search products |
| process | parameters | localhtml | Local name of html file to seach for urls |
| process | parameters | regex | Regular expression pattern to look for (python package regex) |
| process | parameters | product | Copernicus product to download |
| process | parameters | version | Copernicus product version to download |
| process | dstpath | dat | Copernicus raw data file type data |
| process | dstpath | hdr | Copernicus raw data file type header |
| process | dstpath | volume | Source volume with Copernicus data |

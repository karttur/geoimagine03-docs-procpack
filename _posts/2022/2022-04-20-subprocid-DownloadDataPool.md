---
layout: subprocess
categories: subprocess
title: DownloadDataPool
processurl: subprocid-DownloadDataPool
rootprocid: MODISProc
subprocid: DownloadDataPool
author: thomasg
excerpt: Download MODIS tile data from MODIS datapool
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
      "processid": "DownloadDataPool",
      "parameters": {
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
      "processid": "DownloadDataPool",
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
| process | parameters | product | text | True | MCD43A4 |
| process | parameters | version | text | True | 006 |
| process | dstpath | dat | text | False | hdf |
| process | dstpath | hdr | text | False | hdf |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | product | MODIS product to download |
| process | parameters | version | MODIS product version to download |
| process | dstpath | dat | MODIS raw data file type data |
| process | dstpath | hdr | MODIS raw data file type header |
| process | dstpath | volume | Source volume with MODIS data |

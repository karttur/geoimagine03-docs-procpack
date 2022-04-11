---
layout: subprocess
categories: subprocess
title: DownloadModisRegionTiles
processurl: subprocid-DownloadModisRegionTiles
rootprocid: MODISProc
subprocid: DownloadModisRegionTiles
author: thomasg
excerpt: Download MODIS tile data from MODIS datapool
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
      "processid": "DownloadModisRegionTiles",
      "parameters": {
        "remoteuser": "",
        "serverurl": "https://e4ftl01.cr.usgs.gov",
        "asscript": "True",
        "searchdone": "False",
        "temporaldisplacement": "0",
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
      "processid": "DownloadModisRegionTiles",
      "parameters": {
        "remoteuser": "",
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
| process | parameters | remoteuser | string | True | --- |
| process | parameters | serverurl | string | False | https://e4ftl01.cr.usgs.gov |
| process | parameters | asscript | string | False | True |
| process | parameters | searchdone | boolean | False | False |
| process | parameters | temporaldisplacement | integer | False | 0 |
| process | parameters | product | text | True | MCD43A4 |
| process | parameters | version | text | True | 006 |
| process | dstpath | volume | text | True | --- |

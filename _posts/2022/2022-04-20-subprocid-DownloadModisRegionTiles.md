---
layout: subprocess
categories: subprocess
title: DownloadModisRegionTiles
processurl: subprocid-DownloadModisRegionTiles
rootprocid: MODISProc
subprocid: DownloadModisRegionTiles
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

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | remoteuser | Remote user on server with MODIS data |
| process | parameters | serverurl | Remote server with MODIS data |
| process | parameters | asscript | Output as script of direct download |
| process | parameters | searchdone | Search for already downloaded |
| process | parameters | temporaldisplacement | The relative doy to search for particular date |
| process | parameters | product | MODIS product to download |
| process | parameters | version | MODIS product version to download |
| process | dstpath | volume | Destination volume for download |

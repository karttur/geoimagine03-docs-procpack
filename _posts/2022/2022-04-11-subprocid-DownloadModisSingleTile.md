---
layout: subprocess
categories: subprocess
title: DownloadModisSingleTile
processurl: subprocid-DownloadModisSingleTile
rootprocid: MODISProc
subprocid: DownloadModisSingleTile
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
      "processid": "DownloadModisSingleTile",
      "parameters": {
        "remoteuser": "",
        "serverurl": "https://e4ftl01.cr.usgs.gov",
        "asscript": "True",
        "searchdone": "False",
        "product": "MCD43A4",
        "version": "006",
        "xtile": "",
        "ytile": ""
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
      "processid": "DownloadModisSingleTile",
      "parameters": {
        "remoteuser": "",
        "product": "MCD43A4",
        "version": "006",
        "xtile": "",
        "ytile": ""
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
| process | parameters | product | text | True | MCD43A4 |
| process | parameters | version | text | True | 006 |
| process | parameters | xtile | integer | True | --- |
| process | parameters | ytile | integer | True | --- |
| process | dstpath | volume | text | True | --- |

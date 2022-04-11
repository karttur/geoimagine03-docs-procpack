---
layout: subprocess
categories: subprocess
title: DownloadModisSingleTile
processurl: subprocid-DownloadModisSingleTile
rootprocid: MODISProc
subprocid: DownloadModisSingleTile
author: thomasg
excerpt: Download MODIS tile data from MODIS datapool
date: 2022-04-10
modified: 2022-04-10
comments: true
share: true
---


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

---
layout: subprocess
categories: subprocess
title: UnZipRawData
processurl: subprocid-UnZipRawData
rootprocid: Ancillary
subprocid: UnZipRawData
author: thomasg
excerpt: Search local geojson file for tiles to unzip
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
      "processid": "UnZipRawData",
      "parameters": {
        "getlist": "csvfile-getpath1",
        "pattern": "",
        "patternreplace": "pattern",
        "zipreplace": ".tif",
        "srcdir": "",
        "dstdir": "",
        "minlon": "-180",
        "minlat": "-90",
        "maxlon": "180",
        "maxlat": "90"
      },
      "dstpath": {
        "volume": ""
      }
    }
  ]
}
```

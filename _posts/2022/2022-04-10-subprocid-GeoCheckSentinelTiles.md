---
layout: subprocess
categories: subprocess
title: GeoCheckSentinelTiles
processurl: subprocid-GeoCheckSentinelTiles
rootprocid: SentinelProcess
subprocid: GeoCheckSentinelTiles
author: thomasg
excerpt: Check geolocation of sentinel tile
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
      "processid": "GeoCheckSentinelTiles",
      "parameters": {
        "orbitdirection": "B",
        "platformname": "Sentinel-2",
        "prodtype": "S2MSI1C"
      },
      "srcpath": {
        "dat": "tif",
        "hdr": "tif",
        "volume": ""
      }
    }
  ]
}
```

---
layout: subprocess
categories: subprocess
title: ExplodeSentinel
processurl: subprocid-ExplodeSentinel
rootprocid: SentinelProcess
subprocid: ExplodeSentinel
author: thomasg
excerpt: Explode Sentinel tiles
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
      "processid": "ExplodeSentinel",
      "parameters": {
        "granuleoverlap": "0.1",
        "orbitdirection": "B",
        "platformname": "Sentinel-2",
        "exploded": "N",
        "prodtype": "S2MSI1C",
        "cloudmax": "0",
        "setcloudmask": "True",
        "setdetfoomask": "True",
        "setnodatamask": "True",
        "setdefectask": "True",
        "setsaturamask": "True",
        "settecquamask": "False",
        "set0tonull": "True"
      },
      "srcpath": {
        "dat": "zip",
        "hdr": "zip",
        "volume": ""
      },
      "dstpath": {
        "dat": "tif",
        "hdr": "tif",
        "volume": ""
      }
    }
  ]
}
```

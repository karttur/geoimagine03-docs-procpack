---
layout: subprocess
categories: subprocess
title: ExtractModisPolarHdf
processurl: subprocid-ExtractModisPolarHdf
rootprocid: ModisPolar
subprocid: ExtractModisPolarHdf
author: thomasg
excerpt: Extracts the content of modis NSIDC data>
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
      "processid": "ExtractModisPolarHdf",
      "parameters": {
        "asscript": "True",
        "product": "MYD29E1D",
        "version": "006"
      },
      "srcpath": {
        "dat": "",
        "hdr": "hdf",
        "volume": ""
      },
      "dstpath": {
        "dat": "",
        "hdr": "tif",
        "volume": ""
      }
    }
  ]
}
```

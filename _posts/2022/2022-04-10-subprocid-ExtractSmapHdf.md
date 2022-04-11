---
layout: subprocess
categories: subprocess
title: ExtractSmapHdf
processurl: subprocid-ExtractSmapHdf
rootprocid: SmapProc
subprocid: ExtractSmapHdf
author: thomasg
excerpt: Extracts the content of SMAP HDF>
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
      "processid": "ExtractSmapHdf",
      "parameters": {
        "asscript": "True",
        "product": "MYD29E1D",
        "version": "006",
        "remoteuser": "",
        "serverurl": "https://n5eil01u.ecs.nsidc.org",
        "searchdone": "True"
      },
      "srcpath": {
        "dat": "",
        "hdr": "h5",
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

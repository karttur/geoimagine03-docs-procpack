---
layout: subprocess
categories: subprocess
title: SearchUSGSProducts
processurl: subprocid-SearchUSGSProducts
rootprocid: USGSProc
subprocid: SearchUSGSProducts
author: thomasg
excerpt: Access available files in Data pool holding
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
      "processid": "SearchUSGSProducts",
      "parameters": {
        "product": "MCD43A4",
        "version": "006",
        "serverurl": "https://e4ftl01.cr.usgs.gov"
      },
      "dstpath": {
        "volume": ""
      }
    }
  ]
}
```

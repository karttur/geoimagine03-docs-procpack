---
layout: subprocess
categories: subprocess
title: DefineCustomSystem
processurl: subprocid-DefineCustomSystem
rootprocid: ManageRegion
subprocid: DefineCustomSystem
author: thomasg
excerpt: Define a custom system
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
      "processid": "DefineCustomSystem",
      "parameters": {
        "systemid": "slick",
        "epsg": "0",
        "minx": "0",
        "maxx": "0",
        "miny": "0",
        "maxy": "0",
        "xtiles": "0",
        "ytiles": "0",
        "removenoneearthttiles": "False"
      }
    }
  ]
}
```

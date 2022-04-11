---
layout: subprocess
categories: subprocess
title: ModisSearchToDB
processurl: subprocid-ModisSearchToDB
rootprocid: MODISProc
subprocid: ModisSearchToDB
author: thomasg
excerpt: Transfer the MODIS seanch results to the postgres DB
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
      "processid": "ModisSearchToDB",
      "parameters": {
        "remoteuser": "",
        "product": "MCD43A4",
        "version": "006",
        "searchdone": "False"
      },
      "srcpath": {
        "volume": ""
      }
    }
  ]
}
```

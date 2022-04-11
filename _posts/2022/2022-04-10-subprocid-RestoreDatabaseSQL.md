---
layout: subprocess
categories: subprocess
title: RestoreDatabaseSQL
processurl: subprocid-RestoreDatabaseSQL
rootprocid: DatabaseProc
subprocid: RestoreDatabaseSQL
author: thomasg
excerpt: Restore Database
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
      "processid": "RestoreDatabaseSQL",
      "parameters": {
        "host": "localhost",
        "format": "c",
        "cmdpath": "None",
        "dataonly": "false",
        "definitiononly": "false",
        "datum": "0"
      },
      "srcpath": {
        "hdr": "sql",
        "volume": ""
      }
    }
  ]
}
```

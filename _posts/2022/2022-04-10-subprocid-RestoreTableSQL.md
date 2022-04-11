---
layout: subprocess
categories: subprocess
title: RestoreTableSQL
processurl: subprocid-RestoreTableSQL
rootprocid: DatabaseProc
subprocid: RestoreTableSQL
author: thomasg
excerpt: Restore Database table
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
      "processid": "RestoreTableSQL",
      "parameters": {
        "host": "localhost",
        "schema": "system",
        "table": "regions",
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

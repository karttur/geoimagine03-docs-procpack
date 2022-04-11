---
layout: subprocess
categories: subprocess
title: RestoreSchemaSQL
processurl: subprocid-RestoreSchemaSQL
rootprocid: DatabaseProc
subprocid: RestoreSchemaSQL
author: thomasg
excerpt: Restore Database schema
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
      "processid": "RestoreSchemaSQL",
      "parameters": {
        "host": "localhost",
        "schema": "system",
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

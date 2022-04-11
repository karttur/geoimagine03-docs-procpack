---
layout: subprocess
categories: subprocess
title: DumpSchemaSQL
processurl: subprocid-DumpSchemaSQL
rootprocid: DatabaseProc
subprocid: DumpSchemaSQL
author: thomasg
excerpt: Dump Database schema
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
      "processid": "DumpSchemaSQL",
      "parameters": {
        "host": "localhost",
        "schema": "system",
        "format": "c",
        "cmdpath": "None",
        "dataonly": "false",
        "definitiononly": "false"
      },
      "dstpath": {
        "hdr": "sql",
        "volume": ""
      }
    }
  ]
}
```

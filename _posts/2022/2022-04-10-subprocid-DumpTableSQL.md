---
layout: subprocess
categories: subprocess
title: DumpTableSQL
processurl: subprocid-DumpTableSQL
rootprocid: DatabaseProc
subprocid: DumpTableSQL
author: thomasg
excerpt: Dump Database table
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
      "processid": "DumpTableSQL",
      "parameters": {
        "host": "localhost",
        "schema": "system",
        "table": "regions",
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

---
layout: subprocess
categories: subprocess
title: DumpDatabaseSQL
processurl: subprocid-DumpDatabaseSQL
rootprocid: DatabaseProc
subprocid: DumpDatabaseSQL
author: thomasg
excerpt: Dump Database
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
      "processid": "DumpDatabaseSQL",
      "parameters": {
        "host": "localhost",
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

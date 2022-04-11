---
layout: subprocess
categories: subprocess
title: ExportSchemaCsv
processurl: subprocid-ExportSchemaCsv
rootprocid: DatabaseProc
subprocid: ExportSchemaCsv
author: thomasg
excerpt: Export Db schema as individual tables with csv
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
      "processid": "ExportSchemaCsv",
      "parameters": {
        "schema": "system"
      },
      "dstpath": {
        "hdr": "sql",
        "volume": ""
      }
    }
  ]
}
```

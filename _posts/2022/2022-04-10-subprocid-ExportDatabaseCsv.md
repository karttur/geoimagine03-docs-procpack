---
layout: subprocess
categories: subprocess
title: ExportDatabaseCsv
processurl: subprocid-ExportDatabaseCsv
rootprocid: DatabaseProc
subprocid: ExportDatabaseCsv
author: thomasg
excerpt: Export Db as individual tables with csv
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
      "processid": "ExportDatabaseCsv",
      "parameters": {
        "dummy": "None"
      },
      "dstpath": {
        "hdr": "sql",
        "volume": ""
      }
    }
  ]
}
```

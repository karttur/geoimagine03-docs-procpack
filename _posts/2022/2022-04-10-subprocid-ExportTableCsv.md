---
layout: subprocess
categories: subprocess
title: ExportTableCsv
processurl: subprocid-ExportTableCsv
rootprocid: DatabaseProc
subprocid: ExportTableCsv
author: thomasg
excerpt: Export Db table as csv
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
      "processid": "ExportTableCsv",
      "parameters": {
        "schema": "system",
        "table": "regions",
        "columns": "*",
        "wherestatement": ""
      },
      "dstpath": {
        "hdr": "csv",
        "volume": ""
      }
    }
  ]
}
```

---
layout: subprocess
categories: subprocess
title: CopyTableCsv
processurl: subprocid-CopyTableCsv
rootprocid: DatabaseProc
subprocid: CopyTableCsv
author: thomasg
excerpt: COPY Db records for table from csv
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
      "processid": "CopyTableCsv",
      "parameters": {
        "schema": "system",
        "table": "regions",
        "datum": "0"
      },
      "srcpath": {
        "hdr": "csv",
        "volume": ""
      }
    }
  ]
}
```

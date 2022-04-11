---
layout: subprocess
categories: subprocess
title: InsertDatabaseCsv
processurl: subprocid-InsertDatabaseCsv
rootprocid: DatabaseProc
subprocid: InsertDatabaseCsv
author: thomasg
excerpt: Insert indivudual Db records for table from csv
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
      "processid": "InsertDatabaseCsv",
      "parameters": {
        "schema": "system",
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

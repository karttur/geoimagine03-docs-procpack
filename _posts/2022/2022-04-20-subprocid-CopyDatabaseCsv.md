---
layout: subprocess
categories: subprocess
title: CopyDatabaseCsv
processurl: subprocid-CopyDatabaseCsv
rootprocid: DatabaseProc
subprocid: CopyDatabaseCsv
author: thomasg
excerpt: COPY Db records for table from csv
date: 2022-04-20
modified: 2022-04-20
comments: true
share: true
---

#### Complete json command structure (overriding defaults)
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
      "processid": "CopyDatabaseCsv",
      "parameters": {
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
#### Required json command structure (accepting all defaults)
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
      "processid": "CopyDatabaseCsv",
      "parameters": {},
      "srcpath": {
        "volume": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | datum | text | False | 0 |
| process | srcpath | hdr | text | False | csv |
| process | srcpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | datum | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | volume | to be completed |

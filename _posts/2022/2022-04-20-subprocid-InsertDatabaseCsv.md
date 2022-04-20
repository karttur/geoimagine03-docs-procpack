---
layout: subprocess
categories: subprocess
title: InsertDatabaseCsv
processurl: subprocid-InsertDatabaseCsv
rootprocid: DatabaseProc
subprocid: InsertDatabaseCsv
author: thomasg
excerpt: Insert indivudual Db records for table from csv
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
      "processid": "InsertDatabaseCsv",
      "parameters": {
        "schema": "system"
      },
      "srcpath": {
        "volume": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | schema | text | True | system |
| process | parameters | datum | text | False | 0 |
| process | srcpath | hdr | text | False | csv |
| process | srcpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | schema | to be completed |
| process | parameters | datum | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | volume | to be completed |

---
layout: subprocess
categories: subprocess
title: CopyTableCsv
processurl: subprocid-CopyTableCsv
rootprocid: DatabaseProc
subprocid: CopyTableCsv
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
      "processid": "CopyTableCsv",
      "parameters": {
        "schema": "system",
        "table": "regions"
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
| process | parameters | table | text | True | regions |
| process | parameters | datum | text | False | 0 |
| process | srcpath | hdr | text | False | csv |
| process | srcpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | schema | to be completed |
| process | parameters | table | to be completed |
| process | parameters | datum | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | volume | to be completed |

---
layout: subprocess
categories: subprocess
title: ExportTableCsv
processurl: subprocid-ExportTableCsv
rootprocid: DatabaseProc
subprocid: ExportTableCsv
author: thomasg
excerpt: Export Db table as csv
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
      "processid": "ExportTableCsv",
      "parameters": {
        "schema": "system",
        "table": "regions"
      },
      "dstpath": {
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
| process | parameters | columns | text | False | * |
| process | parameters | wherestatement | text | False | --- |
| process | dstpath | hdr | text | False | csv |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | schema | to be completed |
| process | parameters | table | to be completed |
| process | parameters | columns | list of columns to include, set * to include all |
| process | parameters | wherestatement | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | volume | to be completed |

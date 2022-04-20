---
layout: subprocess
categories: subprocess
title: ExportSchemaCsv
processurl: subprocid-ExportSchemaCsv
rootprocid: DatabaseProc
subprocid: ExportSchemaCsv
author: thomasg
excerpt: Export Db schema as individual tables with csv
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
      "processid": "ExportSchemaCsv",
      "parameters": {
        "schema": "system"
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
| process | dstpath | hdr | text | False | sql |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | schema | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | volume | to be completed |

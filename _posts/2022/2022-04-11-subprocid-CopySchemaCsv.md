---
layout: subprocess
categories: subprocess
title: CopySchemaCsv
processurl: subprocid-CopySchemaCsv
rootprocid: DatabaseProc
subprocid: CopySchemaCsv
author: thomasg
excerpt: COPY Db records for table from csv
date: 2022-04-11
modified: 2022-04-11
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
      "processid": "CopySchemaCsv",
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
      "processid": "CopySchemaCsv",
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

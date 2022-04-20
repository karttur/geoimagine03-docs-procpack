---
layout: subprocess
categories: subprocess
title: RestoreTableSQL
processurl: subprocid-RestoreTableSQL
rootprocid: DatabaseProc
subprocid: RestoreTableSQL
author: thomasg
excerpt: Restore Database table
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
      "processid": "RestoreTableSQL",
      "parameters": {
        "host": "localhost",
        "schema": "system",
        "table": "regions",
        "format": "c",
        "cmdpath": "None",
        "dataonly": "false",
        "definitiononly": "false",
        "datum": "0"
      },
      "srcpath": {
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
      "processid": "RestoreTableSQL",
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
| process | parameters | host | text | False | localhost |
| process | parameters | schema | text | True | system |
| process | parameters | table | text | True | regions |
| process | parameters | format | text | False | c |
| process | parameters | cmdpath | text | False | None |
| process | parameters | dataonly | bool | False | false |
| process | parameters | definitiononly | bool | False | false |
| process | parameters | datum | text | False | 0 |
| process | srcpath | hdr | text | False | sql |
| process | srcpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | host | to be completed |
| process | parameters | schema | to be completed |
| process | parameters | table | to be completed |
| process | parameters | format | to be completed |
| process | parameters | cmdpath | to be completed |
| process | parameters | dataonly | to be completed |
| process | parameters | definitiononly | to be completed |
| process | parameters | datum | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | volume | to be completed |

---
layout: subprocess
categories: subprocess
title: DumpTableSQL
processurl: subprocid-DumpTableSQL
rootprocid: DatabaseProc
subprocid: DumpTableSQL
author: thomasg
excerpt: Dump Database table
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
      "processid": "DumpTableSQL",
      "parameters": {
        "host": "localhost",
        "schema": "system",
        "table": "regions",
        "format": "c",
        "cmdpath": "None",
        "dataonly": "false",
        "definitiononly": "false"
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
      "processid": "DumpTableSQL",
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
| process | parameters | host | text | False | localhost |
| process | parameters | schema | text | True | system |
| process | parameters | table | text | True | regions |
| process | parameters | format | text | False | c |
| process | parameters | cmdpath | text | False | None |
| process | parameters | dataonly | bool | False | false |
| process | parameters | definitiononly | bool | False | false |
| process | dstpath | hdr | text | False | sql |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | host | to be completed |
| process | parameters | schema | to be completed |
| process | parameters | table | to be completed |
| process | parameters | format | to be completed |
| process | parameters | cmdpath | to be completed |
| process | parameters | dataonly | to be completed |
| process | parameters | definitiononly | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | volume | to be completed |

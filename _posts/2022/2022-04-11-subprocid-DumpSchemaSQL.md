---
layout: subprocess
categories: subprocess
title: DumpSchemaSQL
processurl: subprocid-DumpSchemaSQL
rootprocid: DatabaseProc
subprocid: DumpSchemaSQL
author: thomasg
excerpt: Dump Database schema
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
      "processid": "DumpSchemaSQL",
      "parameters": {
        "host": "localhost",
        "schema": "system",
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
      "processid": "DumpSchemaSQL",
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
| process | parameters | host | text | False | localhost |
| process | parameters | schema | text | True | system |
| process | parameters | format | text | False | c |
| process | parameters | cmdpath | text | False | None |
| process | parameters | dataonly | bool | False | false |
| process | parameters | definitiononly | bool | False | false |
| process | dstpath | hdr | text | False | sql |
| process | dstpath | volume | text | True | --- |

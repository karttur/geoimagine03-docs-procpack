---
layout: subprocess
categories: subprocess
title: RestoreSchemaSQL
processurl: subprocid-RestoreSchemaSQL
rootprocid: DatabaseProc
subprocid: RestoreSchemaSQL
author: thomasg
excerpt: Restore Database schema
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
      "processid": "RestoreSchemaSQL",
      "parameters": {
        "host": "localhost",
        "schema": "system",
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
      "processid": "RestoreSchemaSQL",
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
| process | parameters | host | text | False | localhost |
| process | parameters | schema | text | True | system |
| process | parameters | format | text | False | c |
| process | parameters | cmdpath | text | False | None |
| process | parameters | dataonly | bool | False | false |
| process | parameters | definitiononly | bool | False | false |
| process | parameters | datum | text | False | 0 |
| process | srcpath | hdr | text | False | sql |
| process | srcpath | volume | text | True | --- |

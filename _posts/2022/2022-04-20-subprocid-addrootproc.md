---
layout: subprocess
categories: subprocess
title: addrootproc
processurl: subprocid-addrootproc
rootprocid: manageprocess
subprocid: addrootproc
author: thomasg
excerpt: Add root process to database
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
      "processid": "addrootproc",
      "parameters": {
        "rootprocid": "",
        "title": "",
        "label": ""
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
      "processid": "addrootproc",
      "parameters": {
        "rootprocid": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | rootprocid | text | True | --- |
| process | parameters | title | text | False | --- |
| process | parameters | label | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | rootprocid | Root process id |
| process | parameters | title | Process title |
| process | parameters | label | Process label |

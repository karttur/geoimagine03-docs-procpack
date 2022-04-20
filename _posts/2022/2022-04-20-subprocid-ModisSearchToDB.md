---
layout: subprocess
categories: subprocess
title: ModisSearchToDB
processurl: subprocid-ModisSearchToDB
rootprocid: MODISProc
subprocid: ModisSearchToDB
author: thomasg
excerpt: Transfer the MODIS seanch results to the postgres DB
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
      "processid": "ModisSearchToDB",
      "parameters": {
        "remoteuser": "",
        "product": "MCD43A4",
        "version": "006",
        "searchdone": "False"
      },
      "srcpath": {
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
      "processid": "ModisSearchToDB",
      "parameters": {
        "remoteuser": "",
        "product": "MCD43A4",
        "version": "006"
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
| process | parameters | remoteuser | text | True | --- |
| process | parameters | product | text | True | MCD43A4 |
| process | parameters | version | text | True | 006 |
| process | parameters | searchdone | Boolean | False | False |
| process | srcpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | remoteuser | to be completed |
| process | parameters | product | MODIS product to load |
| process | parameters | version | MODIS product version to load |
| process | parameters | searchdone | to be completed |
| process | srcpath | volume | source path |

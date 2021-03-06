---
layout: subprocess
categories: subprocess
title: SmapSearchToDB
processurl: subprocid-SmapSearchToDB
rootprocid: SmapProc
subprocid: SmapSearchToDB
author: thomasg
excerpt: Transfer the SMAP seanch results to the postgres DB
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
      "processid": "SmapSearchToDB",
      "parameters": {
        "remoteuser": "",
        "product": "SPL3SMP_E",
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
      "processid": "SmapSearchToDB",
      "parameters": {
        "remoteuser": "",
        "product": "SPL3SMP_E",
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
| process | parameters | product | text | True | SPL3SMP_E |
| process | parameters | version | text | True | 006 |
| process | parameters | searchdone | Boolean | False | False |
| process | srcpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | remoteuser | to be completed |
| process | parameters | product | SMAP product to load |
| process | parameters | version | SMAP product version to load |
| process | parameters | searchdone | to be completed |
| process | srcpath | volume | to be completed |

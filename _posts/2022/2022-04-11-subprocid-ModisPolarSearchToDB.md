---
layout: subprocess
categories: subprocess
title: ModisPolarSearchToDB
processurl: subprocid-ModisPolarSearchToDB
rootprocid: ModisPolar
subprocid: ModisPolarSearchToDB
author: thomasg
excerpt: Transfer the seanch results to the postgres DB
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
      "processid": "ModisPolarSearchToDB",
      "parameters": {
        "remoteuser": "",
        "product": "MYD10A2",
        "version": "006",
        "searchdone": "false"
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
      "processid": "ModisPolarSearchToDB",
      "parameters": {
        "remoteuser": "",
        "product": "MYD10A2",
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
| process | parameters | product | text | True | MYD10A2 |
| process | parameters | version | text | True | 006 |
| process | parameters | searchdone | bool | False | false |
| process | srcpath | volume | text | True | --- |

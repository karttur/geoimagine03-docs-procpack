---
layout: subprocess
categories: subprocess
title: ManageDefRegProj
processurl: subprocid-ManageDefRegProj
rootprocid: ManageProject
subprocid: ManageDefRegProj
author: thomasg
excerpt: Create project
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
      "processid": "ManageDefRegProj",
      "parameters": {
        "defaultregion": "",
        "tractid": "",
        "tractname": "",
        "tracttitle": "",
        "tractlabel": "",
        "projid": "",
        "projname": "",
        "projtitle": "",
        "projlabel": ""
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
      "processid": "ManageDefRegProj",
      "parameters": {
        "defaultregion": "",
        "tractid": "",
        "tractname": "",
        "tracttitle": "",
        "projid": "",
        "projname": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | defaultregion | text | True | --- |
| process | parameters | tractid | text | True | --- |
| process | parameters | tractname | text | True | --- |
| process | parameters | tracttitle | text | True | --- |
| process | parameters | tractlabel | text | False | --- |
| process | parameters | projid | text | True | --- |
| process | parameters | projname | text | True | --- |
| process | parameters | projtitle | text | False | --- |
| process | parameters | projlabel | text | False | --- |

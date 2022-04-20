---
layout: subprocess
categories: subprocess
title: ManageDefRegProj
processurl: subprocid-ManageDefRegProj
rootprocid: ManageProject
subprocid: ManageDefRegProj
author: thomasg
excerpt: Create project
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

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | defaultregion | Select a default region |
| process | parameters | tractid | Set a unique tractid |
| process | parameters | tractname | Tract name |
| process | parameters | tracttitle | Give a title for the tract (for maps) |
| process | parameters | tractlabel | Give a label for the tract |
| process | parameters | projid | Project id (can be the same as the tractid) |
| process | parameters | projname | Project name |
| process | parameters | projtitle | Give a title for the project |
| process | parameters | projlabel | Give a label for the project |

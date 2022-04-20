---
layout: subprocess
categories: subprocess
title: ManageTractProj
processurl: subprocid-ManageTractProj
rootprocid: ManageProject
subprocid: ManageTractProj
author: thomasg
excerpt: Create project from tract
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
      "processid": "ManageTractProj",
      "parameters": {
        "tractid": "",
        "projid": "",
        "projtitle": "",
        "projlabel": "",
        "modtilelink": "False",
        "wrstilelink": "False",
        "mgrstilelink": "False"
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
      "processid": "ManageTractProj",
      "parameters": {
        "tractid": "",
        "projid": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | tractid | text | True | --- |
| process | parameters | projid | text | True | --- |
| process | parameters | projtitle | text | False | --- |
| process | parameters | projlabel | text | False | --- |
| process | parameters | modtilelink | boolean | False | False |
| process | parameters | wrstilelink | boolean | False | False |
| process | parameters | mgrstilelink | boolean | False | False |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | tractid | Select an existing tractid |
| process | parameters | projid | Project id (can be the same as the tractid) |
| process | parameters | projtitle | Give a title for the project |
| process | parameters | projlabel | Give a label for the project |
| process | parameters | modtilelink | MODIS project link |
| process | parameters | wrstilelink | Landsat WRS project link |
| process | parameters | mgrstilelink | Sentinel MGRS project link |

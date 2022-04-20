---
layout: subprocess
categories: subprocess
title: DefineCustomSystem
processurl: subprocid-DefineCustomSystem
rootprocid: ManageRegion
subprocid: DefineCustomSystem
author: thomasg
excerpt: Define a custom system
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
      "processid": "DefineCustomSystem",
      "parameters": {
        "systemid": "slick",
        "epsg": "0",
        "minx": "0",
        "maxx": "0",
        "miny": "0",
        "maxy": "0",
        "xtiles": "0",
        "ytiles": "0",
        "removenoneearthttiles": "False"
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
      "processid": "DefineCustomSystem",
      "parameters": {
        "systemid": "slick",
        "epsg": "0",
        "minx": "0",
        "maxx": "0",
        "miny": "0",
        "maxy": "0",
        "xtiles": "0",
        "ytiles": "0"
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | systemid | string | True | slick |
| process | parameters | epsg | integer | True | 0 |
| process | parameters | minx | float | True | 0 |
| process | parameters | maxx | float | True | 0 |
| process | parameters | miny | float | True | 0 |
| process | parameters | maxy | float | True | 0 |
| process | parameters | xtiles | integer | True | 0 |
| process | parameters | ytiles | integer | True | 0 |
| process | parameters | removenoneearthttiles | boolean | False | False |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | systemid | System identifier for the new system to be creaed |
| process | parameters | epsg | The epsg code for the custom projection syste, |
| process | parameters | minx | to be completed |
| process | parameters | maxx | to be completed |
| process | parameters | miny | to be completed |
| process | parameters | maxy | to be completed |
| process | parameters | xtiles | to be completed |
| process | parameters | ytiles | to be completed |
| process | parameters | removenoneearthttiles | to be completed |

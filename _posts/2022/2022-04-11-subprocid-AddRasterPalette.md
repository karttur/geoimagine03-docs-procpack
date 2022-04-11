---
layout: subprocess
categories: subprocess
title: AddRasterPalette
processurl: subprocid-AddRasterPalette
rootprocid: LayoutProc
subprocid: AddRasterPalette
author: thomasg
excerpt: Add raster palette
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
      "processid": "AddRasterPalette",
      "parameters": {
        "palette": "",
        "compid": "",
        "access": "A",
        "default": "False",
        "setcolor": {
          "user_def_1": {
            "alpha": "0",
            "blue": "0",
            "green": "0",
            "hint": "",
            "id": "0",
            "label": "",
            "red": "0"
          },
          "user_def..n": {
            "alpha": "0",
            "blue": "0",
            "green": "0",
            "hint": "",
            "id": "0",
            "label": "",
            "red": "0"
          }
        }
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
      "processid": "AddRasterPalette",
      "parameters": {
        "palette": "",
        "compid": "",
        "setcolor": {
          "user_def_1": {
            "alpha": "0",
            "blue": "0",
            "green": "0",
            "hint": "",
            "id": "0",
            "label": "",
            "red": "0"
          },
          "user_def..n": {
            "alpha": "0",
            "blue": "0",
            "green": "0",
            "hint": "",
            "id": "0",
            "label": "",
            "red": "0"
          }
        }
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | palette | text | True | --- |
| process | parameters | compid | text | True | --- |
| process | parameters | access | text | False | A |
| process | parameters | default | bool | False | False |
| process | parameters | setcolor | element | True | --- |

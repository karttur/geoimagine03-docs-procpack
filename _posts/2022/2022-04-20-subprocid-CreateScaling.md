---
layout: subprocess
categories: subprocess
title: CreateScaling
processurl: subprocid-CreateScaling
rootprocid: LayoutProc
subprocid: CreateScaling
author: thomasg
excerpt: Create legend for raster layer
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
      "processid": "CreateScaling",
      "parameters": {
        "log": "False",
        "power": "0",
        "powerna": "251",
        "mirror0": "False",
        "scalefac": "1",
        "offsetadd": "0",
        "srcmin": "0",
        "srcmax": "0",
        "dstmin": "0",
        "dstmax": "0"
      },
      "comp": [
        {
          "user_def_id_1": {
            "content": "",
            "id": "",
            "layerid": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def_id..n": {
            "content": "",
            "id": "",
            "layerid": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        }
      ]
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
      "processid": "CreateScaling",
      "parameters": {},
      "comp": [
        {
          "user_def_id_1": {
            "content": "",
            "id": "",
            "layerid": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def_id..n": {
            "content": "",
            "id": "",
            "layerid": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        }
      ]
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | log | boolean | False | False |
| process | parameters | power | real | False | 0 |
| process | parameters | powerna | integer | False | 251 |
| process | parameters | mirror0 | boolean | False | False |
| process | parameters | scalefac | real | False | 1 |
| process | parameters | offsetadd | real | False | 0 |
| process | parameters | srcmin | real | False | 0 |
| process | parameters | srcmax | real | False | 0 |
| process | parameters | dstmin | real | False | 0 |
| process | parameters | dstmax | real | False | 0 |
| process | comp | content | text | True | --- |
| process | comp | id | text | True | --- |
| process | comp | layerid | text | True | --- |
| process | comp | product | text | True | --- |
| process | comp | source | text | True | --- |
| process | comp | suffix | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | log | to be completed |
| process | parameters | power | to be completed |
| process | parameters | powerna | to be completed |
| process | parameters | mirror0 | to be completed |
| process | parameters | scalefac | to be completed |
| process | parameters | offsetadd | to be completed |
| process | parameters | srcmin | to be completed |
| process | parameters | srcmax | to be completed |
| process | parameters | dstmin | to be completed |
| process | parameters | dstmax | to be completed |
| process | comp | content | to be completed |
| process | comp | id | to be completed |
| process | comp | layerid | to be completed |
| process | comp | product | to be completed |
| process | comp | source | to be completed |
| process | comp | suffix | to be completed |

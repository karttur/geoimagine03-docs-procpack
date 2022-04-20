---
layout: subprocess
categories: subprocess
title: AddPubText
processurl: subprocid-AddPubText
rootprocid: LayoutProc
subprocid: AddPubText
author: thomasg
excerpt: Add raster palette
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
      "processid": "AddPubText",
      "parameters": {
        "compid": "",
        "palversion": "0",
        "product": "0",
        "suffix": "0",
        "title": "",
        "header": "",
        "subheader": "",
        "legendheader": "",
        "legendtype": "",
        "banner": "",
        "hints": "",
        "acknow": "",
        "descript": "",
        "reference": "",
        "disclaim": "",
        "copyrigth": ""
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
      "processid": "AddPubText",
      "parameters": {
        "compid": "",
        "palversion": "0",
        "product": "0",
        "suffix": "0",
        "title": "",
        "header": "",
        "subheader": "",
        "legendheader": "",
        "legendtype": "",
        "banner": "",
        "hints": "",
        "acknow": "",
        "descript": "",
        "reference": "",
        "disclaim": "",
        "copyrigth": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | compid | text | True | --- |
| process | parameters | palversion | integer | True | 0 |
| process | parameters | product | integer | True | 0 |
| process | parameters | suffix | integer | True | 0 |
| process | parameters | title | string | True | --- |
| process | parameters | header | string | True | --- |
| process | parameters | subheader | string | True | --- |
| process | parameters | legendheader | string | True | --- |
| process | parameters | legendtype | string | True | --- |
| process | parameters | banner | string | True | --- |
| process | parameters | hints | string | True | --- |
| process | parameters | acknow | string | True | --- |
| process | parameters | descript | string | True | --- |
| process | parameters | reference | string | True | --- |
| process | parameters | disclaim | string | True | --- |
| process | parameters | copyrigth | string | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | compid | to be completed |
| process | parameters | palversion | to be completed |
| process | parameters | product | to be completed |
| process | parameters | suffix | to be completed |
| process | parameters | title | to be completed |
| process | parameters | header | to be completed |
| process | parameters | subheader | to be completed |
| process | parameters | legendheader | to be completed |
| process | parameters | legendtype | to be completed |
| process | parameters | banner | to be completed |
| process | parameters | hints | to be completed |
| process | parameters | acknow | to be completed |
| process | parameters | descript | to be completed |
| process | parameters | reference | to be completed |
| process | parameters | disclaim | to be completed |
| process | parameters | copyrigth | to be completed |

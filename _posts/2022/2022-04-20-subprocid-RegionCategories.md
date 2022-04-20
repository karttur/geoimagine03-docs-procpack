---
layout: subprocess
categories: subprocess
title: RegionCategories
processurl: subprocid-RegionCategories
rootprocid: ManageRegion
subprocid: RegionCategories
author: thomasg
excerpt: Define default region categories for public use
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
      "processid": "RegionCategories",
      "parameters": {
        "regioncat": "",
        "parentcat": "",
        "stratum": "0",
        "title": "",
        "label": ""
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
      "processid": "RegionCategories",
      "parameters": {
        "regioncat": "",
        "parentcat": "",
        "stratum": "0",
        "title": "",
        "label": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | regioncat | text | True | --- |
| process | parameters | parentcat | text | True | --- |
| process | parameters | stratum | integer | True | 0 |
| process | parameters | title | text | True | --- |
| process | parameters | label | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | regioncat | Region category |
| process | parameters | parentcat | Region parent category |
| process | parameters | stratum | Minimum stratum for access |
| process | parameters | title | Region category title |
| process | parameters | label | Region category label |

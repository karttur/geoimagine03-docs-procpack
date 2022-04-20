---
layout: subprocess
categories: subprocess
title: SearchModisPolarProducts
processurl: subprocid-SearchModisPolarProducts
rootprocid: ModisPolar
subprocid: SearchModisPolarProducts
author: thomasg
excerpt: Modis access available files in NSIDC holdings
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
      "processid": "SearchModisPolarProducts",
      "parameters": {
        "product": "MYD10A2",
        "version": "006",
        "serverurl": "https://n5eil01u.ecs.nsidc.org"
      },
      "dstpath": {
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
      "processid": "SearchModisPolarProducts",
      "parameters": {
        "product": "MYD10A2",
        "version": "006",
        "serverurl": "https://n5eil01u.ecs.nsidc.org"
      },
      "dstpath": {
        "volume": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | product | text | True | MYD10A2 |
| process | parameters | version | text | True | 006 |
| process | parameters | serverurl | text | True | https://n5eil01u.ecs.nsidc.org |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | product | to be completed |
| process | parameters | version | to be completed |
| process | parameters | serverurl | to be completed |
| process | dstpath | volume | to be completed |

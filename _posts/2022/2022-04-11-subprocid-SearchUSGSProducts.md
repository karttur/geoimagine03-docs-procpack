---
layout: subprocess
categories: subprocess
title: SearchUSGSProducts
processurl: subprocid-SearchUSGSProducts
rootprocid: USGSProc
subprocid: SearchUSGSProducts
author: thomasg
excerpt: Access available files in Data pool holding
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
      "processid": "SearchUSGSProducts",
      "parameters": {
        "product": "MCD43A4",
        "version": "006",
        "serverurl": "https://e4ftl01.cr.usgs.gov"
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
      "processid": "SearchUSGSProducts",
      "parameters": {
        "product": "MCD43A4",
        "version": "006"
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
| process | parameters | product | text | True | MCD43A4 |
| process | parameters | version | text | True | 006 |
| process | parameters | serverurl | text | False | https://e4ftl01.cr.usgs.gov |
| process | dstpath | volume | text | True | --- |

---
layout: subprocess
categories: subprocess
title: SearchCopernicusProducts
processurl: subprocid-SearchCopernicusProducts
rootprocid: CopernicusProc
subprocid: SearchCopernicusProducts
author: thomasg
excerpt: Access available files in Copernicus holding
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
      "processid": "SearchCopernicusProducts",
      "parameters": {
        "product": "",
        "version": "",
        "serverurl": "gisco-services.ec.europa.eu",
        "remoteuser": "None",
        "password": "None"
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
      "processid": "SearchCopernicusProducts",
      "parameters": {
        "product": "",
        "version": ""
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
| process | parameters | product | text | True | --- |
| process | parameters | version | text | True | --- |
| process | parameters | serverurl | text | False | gisco-services.ec.europa.eu |
| process | parameters | remoteuser | text | False | None |
| process | parameters | password | text | False | None |
| process | dstpath | volume | text | True | --- |

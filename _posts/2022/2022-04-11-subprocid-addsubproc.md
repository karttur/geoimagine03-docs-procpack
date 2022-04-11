---
layout: subprocess
categories: subprocess
title: addsubproc
processurl: subprocid-addsubproc
rootprocid: manageprocess
subprocid: addsubproc
author: thomasg
excerpt: Add sub process to database
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
      "processid": "addsubproc",
      "procsys": {
        "dstdivision": "",
        "dstsystem": "",
        "srcdivision": "",
        "srcsystem": "",
        "system": ""
      },
      "parameters": {
        "rootprocid": "",
        "subprocid": "",
        "version": "",
        "minuserstratum": "1",
        "title": "",
        "label": ""
      },
      "system": {
        "procsys": {
          "dstdivision": "",
          "dstsystem": "",
          "srcdivision": "",
          "srcsystem": "",
          "system": ""
        }
      },
      "node": {
        "element": "",
        "parameter": {
          "defaultvalue": "",
          "paramid": "",
          "paramtyp": "",
          "required": ""
        },
        "parent": ""
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
      "processid": "addsubproc",
      "procsys": {
        "dstdivision": "",
        "dstsystem": "",
        "srcdivision": "",
        "srcsystem": "",
        "system": ""
      },
      "parameters": {
        "rootprocid": "",
        "subprocid": "",
        "version": "",
        "minuserstratum": "1"
      },
      "system": {
        "procsys": {
          "dstdivision": "",
          "dstsystem": "",
          "srcdivision": "",
          "srcsystem": "",
          "system": ""
        }
      },
      "node": {
        "element": "",
        "parameter": {
          "defaultvalue": "",
          "paramid": "",
          "paramtyp": "",
          "required": ""
        },
        "parent": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| system | procsys | dstdivision | text | True | --- |
| system | procsys | dstsystem | text | True | --- |
| system | procsys | srcdivision | text | True | --- |
| system | procsys | srcsystem | text | True | --- |
| system | procsys | system | text | True | --- |

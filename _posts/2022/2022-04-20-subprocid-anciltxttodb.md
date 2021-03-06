---
layout: subprocess
categories: subprocess
title: anciltxttodb
processurl: subprocid-anciltxttodb
rootprocid: Ancillary
subprocid: anciltxttodb
author: thomasg
excerpt: Register ancillary text data in db
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
      "processid": "anciltxttodb",
      "parameters": {
        "schema": "",
        "table": "",
        "template": ""
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "txt",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "txt",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        }
      ],
      "srcpath": {
        "dat": "",
        "hdr": "",
        "volume": ""
      },
      "link": {
        "csvaltcolumn": "-99",
        "csvaltnodata": "",
        "csvcolumn": "",
        "csvnodata": "",
        "dbcolumn": "",
        "format": ""
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
      "processid": "anciltxttodb",
      "parameters": {
        "schema": "",
        "table": "",
        "template": ""
      },
      "srccomp": [
        {
          "user_def_1": {}
        },
        {
          "user_def..n": {}
        }
      ],
      "srcpath": {
        "hdr": "",
        "volume": ""
      },
      "link": {
        "csvcolumn": "",
        "dbcolumn": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | schema | text | True | --- |
| process | parameters | table | text | True | --- |
| process | parameters | template | text | True | --- |
| process | srccomp | element | text | False | * |
| process | srccomp | parent | text | False | process |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | True | --- |
| process | srcpath | volume | text | True | --- |
| process | link | csvaltcolumn | int | False | -99 |
| process | link | csvaltnodata | text | False | --- |
| process | link | csvcolumn | int | True | --- |
| process | link | csvnodata | text | False | --- |
| process | link | dbcolumn | text | True | --- |
| process | link | format | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | schema | to be completed |
| process | parameters | table | to be completed |
| process | parameters | template | to be completed |
| process | srccomp | element | to be completed |
| process | srccomp | parent | to be completed |
| process | srcpath | dat | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | volume | to be completed |
| process | link | csvaltcolumn | to be completed |
| process | link | csvaltnodata | to be completed |
| process | link | csvcolumn | to be completed |
| process | link | csvnodata | to be completed |
| process | link | dbcolumn | to be completed |
| process | link | format | to be completed |

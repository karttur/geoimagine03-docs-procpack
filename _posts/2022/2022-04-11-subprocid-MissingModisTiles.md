---
layout: subprocess
categories: subprocess
title: MissingModisTiles
processurl: subprocid-MissingModisTiles
rootprocid: MODISProc
subprocid: MissingModisTiles
author: thomasg
excerpt: Copies closest neighboring tile to missing
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
      "processid": "MissingModisTiles",
      "parameters": {
        "product": "MCD43A4",
        "version": "006"
      },
      "srccomp": [
        {
          "user_def_1": {}
        },
        {
          "user_def..n": {}
        }
      ],
      "srcband": {
        "id": "",
        "layerid": "",
        "prefix": ""
      },
      "srcpath": {
        "dat": "",
        "hdr": "tif",
        "volume": ""
      },
      "dstpath": {
        "dat": "",
        "hdr": "tif",
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
      "processid": "MissingModisTiles",
      "parameters": {
        "product": "MCD43A4",
        "version": "006"
      },
      "srccomp": [
        {
          "user_def_1": {}
        },
        {
          "user_def..n": {}
        }
      ],
      "srcband": {
        "id": "",
        "layerid": "",
        "prefix": ""
      },
      "srcpath": {
        "hdr": "tif",
        "volume": ""
      },
      "dstpath": {
        "hdr": "tif",
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
| process | srccomp | content | text | True | --- |
| process | srccomp | layerid | text | True | * |
| process | srccomp | masked | bool | False | Y |
| process | srccomp | prefix | text | True | --- |
| process | srccomp | product | text | True | --- |
| process | srccomp | source | text | True | --- |
| process | srccomp | suffix | text | True | --- |
| process | srcband | id | text | True | --- |
| process | srcband | layerid | text | True | --- |
| process | srcband | prefix | text | True | --- |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | True | tif |
| process | srcpath | volume | text | True | --- |
| process | dstpath | dat | text | False | --- |
| process | dstpath | hdr | text | True | tif |
| process | dstpath | volume | text | True | --- |

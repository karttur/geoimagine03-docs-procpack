---
layout: subprocess
categories: subprocess
title: UpdateRasterMeta
processurl: subprocid-UpdateRasterMeta
rootprocid: LayoutProc
subprocid: UpdateRasterMeta
author: thomasg
excerpt: Replace null and color ramp in existing raster
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
      "processid": "UpdateRasterMeta",
      "parameters": {
        "cellnull": "0",
        "celltype": "",
        "scalefac": "0",
        "offsetadd": "0",
        "dataunit": "",
        "palette": ""
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
        "dat": "",
        "hdr": "",
        "volume": ""
      },
      "dstpath": {
        "dat": "",
        "hdr": ""
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
      "processid": "UpdateRasterMeta",
      "parameters": {
        "cellnull": "0"
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
      "dstpath": {
        "hdr": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | cellnull | integer | True | 0 |
| process | parameters | celltype | text | False | --- |
| process | parameters | scalefac | real | False | 0 |
| process | parameters | offsetadd | integer | False | 0 |
| process | parameters | dataunit | text | False | --- |
| process | parameters | palette | text | False | --- |
| process | srccomp | content | text | True | --- |
| process | srccomp | layerid | text | True | src |
| process | srccomp | prefix | text | True | --- |
| process | srccomp | product | text | True | --- |
| process | srccomp | source | text | True | --- |
| process | srccomp | suffix | text | True | --- |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | True | --- |
| process | srcpath | volume | text | True | --- |
| process | dstpath | dat | text | False | --- |
| process | dstpath | hdr | text | True | --- |

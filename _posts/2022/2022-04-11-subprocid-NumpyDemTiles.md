---
layout: subprocess
categories: subprocess
title: NumpyDemTiles
processurl: subprocid-NumpyDemTiles
rootprocid: NumpyProc
subprocid: NumpyDemTiles
author: thomasg
excerpt: Generate DEM derivates
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
      "processid": "NumpyDemTiles",
      "parameters": {
        "mode": "slope",
        "mosaic": "True",
        "radiuscsv": "1",
        "compute_edges": "True",
        "trigonometric": "False",
        "kernelform": "square",
        "kernelvalues": "equal",
        "standardize": "False",
        "tpithreshold": "5",
        "slopethreshold": "1",
        "dtpistd": "25",
        "btpistd": "50",
        "palette": ""
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        }
      ],
      "srcpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      },
      "dstcopy": {
        "dataunit": "auto",
        "layerid": "auto",
        "prefix": "auto",
        "srccomp": "*",
        "suffix": "auto"
      },
      "dstpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
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
      "processid": "NumpyDemTiles",
      "parameters": {
        "mode": "slope"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        }
      ],
      "srcpath": {
        "volume": ""
      },
      "dstcopy": {
        "srccomp": "*"
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
| process | parameters | mode | text | True | slope |
| process | parameters | mosaic | boolean | False | True |
| process | parameters | radiuscsv | text | False | 1 |
| process | parameters | compute_edges | boolean | False | True |
| process | parameters | trigonometric | boolean | False | False |
| process | parameters | kernelform | text | False | square |
| process | parameters | kernelvalues | text | False | equal |
| process | parameters | standardize | boolean | False | False |
| process | parameters | tpithreshold | float | False | 5 |
| process | parameters | slopethreshold | float | False | 1 |
| process | parameters | dtpistd | float | False | 25 |
| process | parameters | btpistd | float | False | 50 |
| process | parameters | palette | text | False | --- |
| process | srccomp | * | element | True | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcopy | dataunit | text | False | auto |
| process | dstcopy | layerid | text | False | auto |
| process | dstcopy | prefix | text | False | auto |
| process | dstcopy | srccomp | text | True | * |
| process | dstcopy | suffix | text | False | auto |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | dat | text | False | --- |

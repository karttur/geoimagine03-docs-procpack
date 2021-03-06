---
layout: subprocess
categories: subprocess
title: OverlayManyToOne
processurl: subprocid-OverlayManyToOne
rootprocid: Overlay
subprocid: OverlayManyToOne
author: thomasg
excerpt: Average Images
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
      "processid": "OverlayManyToOne",
      "parameters": {
        "copycomp": "compto1",
        "version": "1.3",
        "statistic": "average",
        "validfraction": "0.5"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "timeseries",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "timeseries",
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
      "dstcomp": [
        {
          "user_def_1": {
            "content": "src",
            "layerid": "*",
            "prefix": "*",
            "product": "src",
            "source": "src",
            "suffix": "*"
          }
        },
        {
          "user_def..n": {
            "content": "src",
            "layerid": "*",
            "prefix": "*",
            "product": "src",
            "source": "src",
            "suffix": "*"
          }
        }
      ],
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
      "processid": "OverlayManyToOne",
      "parameters": {
        "copycomp": "compto1",
        "statistic": "average"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "timeseries",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "timeseries",
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
      "dstcomp": [
        {
          "user_def_1": {
            "content": "src",
            "layerid": "*",
            "prefix": "*",
            "product": "src",
            "source": "src",
            "suffix": "*"
          }
        },
        {
          "user_def..n": {
            "content": "src",
            "layerid": "*",
            "prefix": "*",
            "product": "src",
            "source": "src",
            "suffix": "*"
          }
        }
      ],
      "dstpath": {
        "volume": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | copycomp | text | True | compto1 |
| process | parameters | version | text | False | 1.3 |
| process | parameters | statistic | text | True | average |
| process | parameters | validfraction | real | False | 0.5 |
| process | srccomp | element | text | False | * |
| process | srccomp | parent | text | False | process |
| process | srccomp | timeseries | element | True | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcomp | * | element | True | * |
| process | dstcomp | element | text | False | * |
| process | dstcomp | parent | text | False | process |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | copycomp | to be completed |
| process | parameters | version | to be completed |
| process | parameters | statistic | to be completed |
| process | parameters | validfraction | to be completed |
| process | srccomp | element | to be completed |
| process | srccomp | parent | to be completed |
| process | srccomp | timeseries | to be completed |
| process | srcpath | volume | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | dat | to be completed |
| process | dstcomp | * | to be completed |
| process | dstcomp | element | to be completed |
| process | dstcomp | parent | to be completed |
| process | dstpath | volume | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | dat | to be completed |

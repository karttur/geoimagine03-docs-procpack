---
layout: subprocess
categories: subprocess
title: NumpyGeomorphology
processurl: subprocid-NumpyGeomorphology
rootprocid: NumpyProc
subprocid: NumpyGeomorphology
author: thomasg
excerpt: Extract Geomorphology from multilayers
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
      "processid": "NumpyGeomorphology",
      "parameters": {
        "mode": "weiss",
        "standardize": "False",
        "detailedTPIstd": "30",
        "bluntTPIstd": "50",
        "slopethreshold": "1",
        "tpithreshold": "5",
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
        "cellnull": "255",
        "celltype": "Byte",
        "dataunit": "class",
        "layerid": "*",
        "prefix": "*",
        "srccomp": "bluntTPI"
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
      "processid": "NumpyGeomorphology",
      "parameters": {
        "mode": "weiss"
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
        "layerid": "*",
        "prefix": "*",
        "srccomp": "bluntTPI"
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
| process | parameters | mode | text | True | weiss |
| process | parameters | standardize | boolean | False | False |
| process | parameters | detailedTPIstd | float | False | 30 |
| process | parameters | bluntTPIstd | float | False | 50 |
| process | parameters | slopethreshold | float | False | 1 |
| process | parameters | tpithreshold | float | False | 5 |
| process | parameters | palette | text | False | --- |
| process | srccomp | bluntTPI | element | True | bluntTPI |
| process | srccomp | detailedTPI | element | True | detailedTPI |
| process | srccomp | slope | element | True | slope |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcopy | cellnull | integer | False | 255 |
| process | dstcopy | celltype | text | False | Byte |
| process | dstcopy | dataunit | text | False | class |
| process | dstcopy | layerid | text | True | * |
| process | dstcopy | prefix | text | True | * |
| process | dstcopy | srccomp | text | True | bluntTPI |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | mode | to be completed |
| process | parameters | standardize | Standardize or not. |
| process | parameters | detailedTPIstd | Global standard deviation for detailed TPI |
| process | parameters | bluntTPIstd | Global standard deviation for blunt TPI |
| process | parameters | slopethreshold | slope threshold |
| process | parameters | tpithreshold | TPI threshold |
| process | parameters | palette | Palette. |
| process | srccomp | bluntTPI | link for source composition blunt TPI |
| process | srccomp | detailedTPI | link for source composition detailed TPI |
| process | srccomp | slope | link for source composition slope |
| process | srcpath | volume | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | dat | to be completed |
| process | dstcopy | cellnull | unknown hint |
| process | dstcopy | celltype | unknown hint |
| process | dstcopy | dataunit | unknown hint |
| process | dstcopy | layerid | unknown hint |
| process | dstcopy | prefix | unknown hint |
| process | dstcopy | srccomp | unknown hint |
| process | dstpath | volume | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | dat | to be completed |

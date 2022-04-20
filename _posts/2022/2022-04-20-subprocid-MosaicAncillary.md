---
layout: subprocess
categories: subprocess
title: MosaicAncillary
processurl: subprocid-MosaicAncillary
rootprocid: Ancillary
subprocid: MosaicAncillary
author: thomasg
excerpt: Mosaic ancillary data
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
      "processid": "MosaicAncillary",
      "parameters": {
        "getlist": "oswalk",
        "srcdir": "",
        "pattern": "",
        "nonpattern": ""
      },
      "srcpath": {
        "dat": "",
        "hdr": "tif",
        "volume": ""
      },
      "dstcomp": [
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
      "dstpath": {
        "dat": "",
        "hdr": "vrt",
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
      "processid": "MosaicAncillary",
      "parameters": {
        "getlist": "oswalk",
        "srcdir": ""
      },
      "srcpath": {
        "volume": ""
      },
      "dstcomp": [
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
      "dstpath": {
        "volume": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | getlist | text | True | oswalk |
| process | parameters | srcdir | text | True | --- |
| process | parameters | pattern | csvlist | False | --- |
| process | parameters | nonpattern | csvlist | False | --- |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | volume | text | True | --- |
| process | dstcomp | * | element | True | * |
| process | dstpath | dat | text | False | --- |
| process | dstpath | hdr | text | False | vrt |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | getlist |  code that identifies which subroutine to use for import |
| process | parameters | srcdir | path where the src tiles are located |
| process | parameters | pattern | list csv search terms for identifying valid tiles |
| process | parameters | nonpattern | list csv search terms for excluding non-valid tiles |
| process | srcpath | dat | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | volume | to be completed |
| process | dstcomp | * | link for destination composition |
| process | dstpath | dat | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | volume | to be completed |

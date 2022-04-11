---
layout: subprocess
categories: subprocess
title: ExportMovieClockLayout
processurl: subprocid-ExportMovieClockLayout
rootprocid: Export
subprocid: ExportMovieClockLayout
author: thomasg
excerpt: Create movieclock layout
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
      "processid": "ExportMovieClockLayout",
      "parameters": {
        "overwriteshade": "False",
        "overwritelayout": "False",
        "width": "900",
        "name": "",
        "asscript": "True",
        "vector": "NA"
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
        "hdr": "png",
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
      "processid": "ExportMovieClockLayout",
      "parameters": {
        "width": "900",
        "name": ""
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
| process | parameters | overwriteshade | boolean | False | False |
| process | parameters | overwritelayout | boolean | False | False |
| process | parameters | width | integer | True | 900 |
| process | parameters | name | text | True | --- |
| process | parameters | asscript | bool | False | True |
| process | parameters | vector | text | False | NA |
| process | dstcomp | * | element | True | * |
| process | dstpath | hdr | text | False | png |
| process | dstpath | volume | text | True | --- |

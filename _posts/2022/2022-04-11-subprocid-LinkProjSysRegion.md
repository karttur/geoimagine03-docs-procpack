---
layout: subprocess
categories: subprocess
title: LinkProjSysRegion
processurl: subprocid-LinkProjSysRegion
rootprocid: ManageRegion
subprocid: LinkProjSysRegion
author: thomasg
excerpt: Link Project System region to system tiles
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
      "processid": "LinkProjSysRegion",
      "parameters": {
        "checkfixvalidity": "False",
        "onlytiling": "False"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "product": "pubroi",
            "source": "karttur",
            "suffix": "v010"
          }
        },
        {
          "user_def..n": {
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "product": "pubroi",
            "source": "karttur",
            "suffix": "v010"
          }
        }
      ],
      "srcpath": {
        "volume": "",
        "hdr": "shp",
        "dat": "shp"
      },
      "dstcomp": [
        {
          "user_def_1": {}
        },
        {
          "user_def..n": {}
        }
      ],
      "dstpath": {
        "volume": "",
        "hdr": "shp",
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
      "processid": "LinkProjSysRegion",
      "parameters": {},
      "srccomp": [
        {
          "user_def_1": {
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "product": "pubroi",
            "source": "karttur",
            "suffix": "v010"
          }
        },
        {
          "user_def..n": {
            "content": "roi",
            "layerid": "defreg",
            "prefix": "defreg",
            "product": "pubroi",
            "source": "karttur",
            "suffix": "v010"
          }
        }
      ],
      "srcpath": {
        "volume": ""
      },
      "dstcomp": [
        {
          "user_def_1": {}
        },
        {
          "user_def..n": {}
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
| process | parameters | checkfixvalidity | bool | False | False |
| process | parameters | onlytiling | boolean | False | False |
| process | srccomp | * | element | True | * |
| process | srccomp | parent | text | False | process |
| process | srccomp | element | text | False | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | shp |
| process | srcpath | dat | text | False | shp |
| process | dstcomp | region | element | True | region |
| process | dstcomp | tiles | element | True | tiles |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | shp |
| process | dstpath | dat | text | False | --- |

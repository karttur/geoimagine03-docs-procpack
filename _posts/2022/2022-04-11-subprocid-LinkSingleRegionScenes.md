---
layout: subprocess
categories: subprocess
title: LinkSingleRegionScenes
processurl: subprocid-LinkSingleRegionScenes
rootprocid: ManageRegion
subprocid: LinkSingleRegionScenes
author: thomasg
excerpt: Link Single Region to system scenes
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
      "processid": "LinkSingleRegionScenes",
      "parameters": {
        "defregmask": "None",
        "wrs": "2",
        "dir": "D",
        "minarea": "0",
        "regionid": "*",
        "regiontype": "default",
        "regioncat": "*"
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
        "dat": "shp",
        "hdr": "shp",
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
      "processid": "LinkSingleRegionScenes",
      "parameters": {
        "regioncat": "*"
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
        "volume": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | defregmask | text | False | None |
| process | parameters | wrs | integer | False | 2 |
| process | parameters | dir | text | False | D |
| process | parameters | minarea | float | False | 0 |
| process | parameters | regionid | text | False | * |
| process | parameters | regiontype | text | False | default |
| process | parameters | regioncat | text | True | * |
| process | srccomp | * | element | True | * |
| process | srccomp | element | text | False | * |
| process | srccomp | parent | text | False | process |
| process | srcpath | dat | text | False | shp |
| process | srcpath | hdr | text | False | shp |
| process | srcpath | volume | text | True | --- |

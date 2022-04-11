---
layout: subprocess
categories: subprocess
title: LinkDefaultRegionScenes
processurl: subprocid-LinkDefaultRegionScenes
rootprocid: ManageRegion
subprocid: LinkDefaultRegionScenes
author: thomasg
excerpt: Link Default Regions to system scenes
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
      "processid": "LinkDefaultRegionScenes",
      "parameters": {
        "defregmask": "land",
        "srcepsgL": "4326",
        "regioncat": "None",
        "regionid": "*",
        "checkfixvalidity": "False",
        "ogr2ogr": "False",
        "cmdpath": "None",
        "clipsrc": "",
        "clipdst": "False",
        "wrapdateline": "True",
        "onlyregionsfullywithinsystem": "True",
        "onlytiling": "False",
        "wrs": "2",
        "dir": "D",
        "minarea": "0"
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
      "processid": "LinkDefaultRegionScenes",
      "parameters": {
        "regioncat": "None"
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
| process | parameters | defregmask | text | False | land |
| process | parameters | srcepsgL | text | False | 4326 |
| process | parameters | regioncat | text | True | None |
| process | parameters | regionid | text | False | * |
| process | parameters | checkfixvalidity | bool | False | False |
| process | parameters | ogr2ogr | boolean | False | False |
| process | parameters | cmdpath | text | False | None |
| process | parameters | clipsrc | text | False | --- |
| process | parameters | clipdst | boolean | False | False |
| process | parameters | wrapdateline | boolean | False | True |
| process | parameters | onlyregionsfullywithinsystem | boolean | False | True |
| process | parameters | onlytiling | boolean | False | False |
| process | parameters | wrs | integer | False | 2 |
| process | parameters | dir | text | False | D |
| process | parameters | minarea | float | False | 0 |
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

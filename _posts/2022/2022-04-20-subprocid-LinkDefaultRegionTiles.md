---
layout: subprocess
categories: subprocess
title: LinkDefaultRegionTiles
processurl: subprocid-LinkDefaultRegionTiles
rootprocid: ManageRegion
subprocid: LinkDefaultRegionTiles
author: thomasg
excerpt: Link Default Regions to system tiles
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
      "processid": "LinkDefaultRegionTiles",
      "parameters": {
        "defregmask": "land",
        "srcepsgL": "4326",
        "regioncat": "None",
        "regionid": "*",
        "checkfixvalidity": "True",
        "ogr2ogr": "False",
        "cmdpath": "None",
        "clipsrc": "",
        "clipdst": "False",
        "wrapdateline": "True",
        "onlyregionsfullywithinsystem": "True",
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
      "processid": "LinkDefaultRegionTiles",
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
| process | parameters | checkfixvalidity | bool | False | True |
| process | parameters | ogr2ogr | boolean | False | False |
| process | parameters | cmdpath | text | False | None |
| process | parameters | clipsrc | text | False | --- |
| process | parameters | clipdst | boolean | False | False |
| process | parameters | wrapdateline | boolean | False | True |
| process | parameters | onlyregionsfullywithinsystem | boolean | False | True |
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

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | defregmask | Default region for restricting tile search |
| process | parameters | srcepsgL | Csv list of srcepsg regions to use for linking - default is 4326 |
| process | parameters | regioncat | to be completed |
| process | parameters | regionid | to be completed |
| process | parameters | checkfixvalidity | check and fix validty of simplifed vector before saving |
| process | parameters | ogr2ogr | to be completed |
| process | parameters | cmdpath | to be completed |
| process | parameters | clipsrc | empty (default) or csv for src minx, miny, maxx, maxy |
| process | parameters | clipdst | to be completed |
| process | parameters | wrapdateline | to be completed |
| process | parameters | onlyregionsfullywithinsystem | to be completed |
| process | parameters | onlytiling | to be completed |
| process | srccomp | * | Hierarchical pointer |
| process | srccomp | parent | to be completed |
| process | srccomp | element | to be completed |
| process | srcpath | volume | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | dat | to be completed |
| process | dstcomp | region | link for destination composition |
| process | dstcomp | tiles | link for destination composition |
| process | dstpath | volume | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | dat | to be completed |

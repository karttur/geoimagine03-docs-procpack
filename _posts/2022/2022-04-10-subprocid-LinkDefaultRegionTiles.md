---
layout: subprocess
categories: subprocess
title: LinkDefaultRegionTiles
processurl: subprocid-LinkDefaultRegionTiles
rootprocid: ManageRegion
subprocid: LinkDefaultRegionTiles
author: thomasg
excerpt: Link Default Regions to system tiles
date: 2022-04-10
modified: 2022-04-10
comments: true
share: true
---


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

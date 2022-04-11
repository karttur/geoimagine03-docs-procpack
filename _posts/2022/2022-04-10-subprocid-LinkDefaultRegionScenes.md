---
layout: subprocess
categories: subprocess
title: LinkDefaultRegionScenes
processurl: subprocid-LinkDefaultRegionScenes
rootprocid: ManageRegion
subprocid: LinkDefaultRegionScenes
author: thomasg
excerpt: Link Default Regions to system scenes
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

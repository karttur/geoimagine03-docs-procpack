---
layout: subprocess
categories: subprocess
title: LinkSingleRegionScenes
processurl: subprocid-LinkSingleRegionScenes
rootprocid: ManageRegion
subprocid: LinkSingleRegionScenes
author: thomasg
excerpt: Link Single Region to system scenes
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

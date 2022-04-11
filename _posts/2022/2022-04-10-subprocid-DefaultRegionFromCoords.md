---
layout: subprocess
categories: subprocess
title: DefaultRegionFromCoords
processurl: subprocid-DefaultRegionFromCoords
rootprocid: ManageRegion
subprocid: DefaultRegionFromCoords
author: thomasg
excerpt: Define default region for public use from corner coordinates
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
      "processid": "DefaultRegionFromCoords",
      "parameters": {
        "regionid": "",
        "regionname": "",
        "regioncat": "",
        "parentid": "",
        "parentcat": "",
        "stratum": "0",
        "minx": "0",
        "maxx": "0",
        "miny": "0",
        "maxy": "0",
        "epsg": "4326",
        "version": "1.0",
        "title": "Title",
        "label": "Label"
      },
      "dstcomp": [
        {
          "user_def_1": {
            "cellnull": "0",
            "celltype": "vector",
            "content": "roi",
            "dataunit": "boundary",
            "layerid": "defreg",
            "masked": "N",
            "measure": "N",
            "offsetadd": "0",
            "prefix": "defreg",
            "product": "pubroi",
            "scalefac": "1",
            "source": "karttur",
            "suffix": "v010"
          }
        },
        {
          "user_def..n": {
            "cellnull": "0",
            "celltype": "vector",
            "content": "roi",
            "dataunit": "boundary",
            "layerid": "defreg",
            "masked": "N",
            "measure": "N",
            "offsetadd": "0",
            "prefix": "defreg",
            "product": "pubroi",
            "scalefac": "1",
            "source": "karttur",
            "suffix": "v010"
          }
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

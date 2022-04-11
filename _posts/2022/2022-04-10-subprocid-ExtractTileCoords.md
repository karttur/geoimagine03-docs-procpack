---
layout: subprocess
categories: subprocess
title: ExtractTileCoords
processurl: subprocid-ExtractTileCoords
rootprocid: ManageRegion
subprocid: ExtractTileCoords
author: thomasg
excerpt: Extract tile coordinates
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
      "processid": "ExtractTileCoords",
      "parameters": {
        "centroid": "True",
        "mgrs": "MGRS",
        "gzd": "GZD",
        "utmzone": "ZONE",
        "wrspath": "PATH",
        "wrsrow": "ROW",
        "wrsmode": "MODE",
        "wrs": "2"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "vector",
            "layerid": "vector",
            "prefix": "vector",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "vector",
            "layerid": "vector",
            "prefix": "vector",
            "product": "",
            "source": "",
            "suffix": ""
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

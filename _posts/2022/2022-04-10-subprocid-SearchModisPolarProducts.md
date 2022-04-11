---
layout: subprocess
categories: subprocess
title: SearchModisPolarProducts
processurl: subprocid-SearchModisPolarProducts
rootprocid: ModisPolar
subprocid: SearchModisPolarProducts
author: thomasg
excerpt: Modis access available files in NSIDC holdings
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
      "processid": "SearchModisPolarProducts",
      "parameters": {
        "product": "MYD10A2",
        "version": "006",
        "serverurl": "https://n5eil01u.ecs.nsidc.org"
      },
      "dstpath": {
        "volume": ""
      }
    }
  ]
}
```

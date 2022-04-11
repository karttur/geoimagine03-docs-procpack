---
layout: subprocess
categories: subprocess
title: OverlayManyToOne
processurl: subprocid-OverlayManyToOne
rootprocid: Overlay
subprocid: OverlayManyToOne
author: thomasg
excerpt: Average Images
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
      "processid": "OverlayManyToOne",
      "parameters": {
        "copycomp": "compto1",
        "version": "1.3",
        "statistic": "average",
        "validfraction": "0.5"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "timeseries",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "timeseries",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        }
      ],
      "srcpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      },
      "dstcomp": [
        {
          "user_def_1": {
            "content": "src",
            "layerid": "*",
            "prefix": "*",
            "product": "src",
            "source": "src",
            "suffix": "*"
          }
        },
        {
          "user_def..n": {
            "content": "src",
            "layerid": "*",
            "prefix": "*",
            "product": "src",
            "source": "src",
            "suffix": "*"
          }
        }
      ],
      "dstpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      }
    }
  ]
}
```

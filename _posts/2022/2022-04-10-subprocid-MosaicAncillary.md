---
layout: subprocess
categories: subprocess
title: MosaicAncillary
processurl: subprocid-MosaicAncillary
rootprocid: Ancillary
subprocid: MosaicAncillary
author: thomasg
excerpt: Mosaic ancillary data
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
      "processid": "MosaicAncillary",
      "parameters": {
        "getlist": "oswalk",
        "srcdir": "",
        "pattern": "",
        "nonpattern": ""
      },
      "srcpath": {
        "dat": "",
        "hdr": "tif",
        "volume": ""
      },
      "dstcomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        }
      ],
      "dstpath": {
        "dat": "",
        "hdr": "vrt",
        "volume": ""
      }
    }
  ]
}
```

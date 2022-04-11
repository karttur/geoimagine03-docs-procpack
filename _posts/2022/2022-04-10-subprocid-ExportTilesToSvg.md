---
layout: subprocess
categories: subprocess
title: ExportTilesToSvg
processurl: subprocid-ExportTilesToSvg
rootprocid: Export
subprocid: ExportTilesToSvg
author: thomasg
excerpt: Export data to SVG
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
      "processid": "ExportTilesToSvg",
      "parameters": {
        "overwriteshade": "False",
        "overwritelayout": "False",
        "tolerance": "0",
        "simplify": "0",
        "scale": "0",
        "dstepsg": "4326",
        "stroke": "black",
        "fill": "none",
        "symbol": "None",
        "strokewidth": "1",
        "strokedasharray": "",
        "padding": "0",
        "pngsize": "",
        "crop": "",
        "asscript": "False"
      },
      "srccomp": [
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
      "srcpath": {
        "volume": "",
        "hdr": "shp",
        "dat": ""
      },
      "dstcopy": {
        "layerid": "copy",
        "prefix": "copy",
        "srccomp": "*",
        "suffix": "copy"
      },
      "dstpath": {
        "volume": "",
        "hdr": "svg",
        "dat": "png"
      }
    }
  ]
}
```

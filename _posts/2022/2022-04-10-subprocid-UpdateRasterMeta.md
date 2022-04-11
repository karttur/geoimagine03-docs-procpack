---
layout: subprocess
categories: subprocess
title: UpdateRasterMeta
processurl: subprocid-UpdateRasterMeta
rootprocid: LayoutProc
subprocid: UpdateRasterMeta
author: thomasg
excerpt: Replace null and color ramp in existing raster
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
      "processid": "UpdateRasterMeta",
      "parameters": {
        "cellnull": "0",
        "celltype": "",
        "scalefac": "0",
        "offsetadd": "0",
        "dataunit": "",
        "palette": ""
      },
      "srccomp": [
        {
          "user_def_1": {}
        },
        {
          "user_def..n": {}
        }
      ],
      "srcpath": {
        "dat": "",
        "hdr": "",
        "volume": ""
      },
      "dstpath": {
        "dat": "",
        "hdr": ""
      }
    }
  ]
}
```

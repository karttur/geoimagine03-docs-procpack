---
layout: subprocess
categories: subprocess
title: NumpyGeomorphology
processurl: subprocid-NumpyGeomorphology
rootprocid: NumpyProc
subprocid: NumpyGeomorphology
author: thomasg
excerpt: Extract Geomorphology from multilayers
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
      "processid": "NumpyGeomorphology",
      "parameters": {
        "mode": "weiss",
        "standardize": "False",
        "detailedTPIstd": "30",
        "bluntTPIstd": "50",
        "slopethreshold": "1",
        "tpithreshold": "5",
        "palette": ""
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
        "hdr": "tif",
        "dat": ""
      },
      "dstcopy": {
        "cellnull": "255",
        "celltype": "Byte",
        "dataunit": "class",
        "layerid": "*",
        "prefix": "*",
        "srccomp": "bluntTPI"
      },
      "dstpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      }
    }
  ]
}
```

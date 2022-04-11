---
layout: subprocess
categories: subprocess
title: DefaultRegionFromVector
processurl: subprocid-DefaultRegionFromVector
rootprocid: ManageRegion
subprocid: DefaultRegionFromVector
author: thomasg
excerpt: Define default region from vector data set
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
      "processid": "DefaultRegionFromVector",
      "parameters": {
        "vector_db_id": "ISO_A3",
        "vector_db_name": "NAME",
        "vector_db_category": "",
        "vector_db_parentid": "PARENTID",
        "vector_db_parentcat": "PARENTCAT",
        "vector_db_stratum": "STRATUM",
        "vector_db_title": "TITLE",
        "vector_db_label": "LABEL",
        "version": "1.0"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "srcdefregvec",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "srcdefregvec",
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
        "dat": "na"
      },
      "dstcopy": {
        "layerid": "*",
        "srccomp": "*"
      },
      "dstpath": {
        "volume": "",
        "hdr": "shp",
        "dat": "na"
      }
    }
  ]
}
```

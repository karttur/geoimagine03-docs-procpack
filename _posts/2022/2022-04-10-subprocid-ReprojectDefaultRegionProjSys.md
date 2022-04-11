---
layout: subprocess
categories: subprocess
title: ReprojectDefaultRegionProjSys
processurl: subprocid-ReprojectDefaultRegionProjSys
rootprocid: ManageRegion
subprocid: ReprojectDefaultRegionProjSys
author: thomasg
excerpt: Reproject default region to predefined projsys
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
      "processid": "ReprojectDefaultRegionProjSys",
      "parameters": {
        "version": "1.3",
        "asscript": "False",
        "src_defregid": "",
        "checkfixvalidity": "True",
        "ogr2ogr": "True",
        "cmdpath": "None",
        "clipdst": "True",
        "tr_xres": "0",
        "tr_yres": "0",
        "resample": "near",
        "celltype": "auto",
        "errorthreshold": "0"
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
        "cellnull": "0",
        "celltype": "vector",
        "dataunit": "boundary",
        "layerid": "*",
        "masked": "N",
        "measure": "N",
        "offsetadd": "0",
        "scalefac": "1",
        "srccomp": "*"
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

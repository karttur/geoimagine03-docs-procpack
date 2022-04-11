---
layout: subprocess
categories: subprocess
title: ReprojectAncillaryRegionProjSys
processurl: subprocid-ReprojectAncillaryRegionProjSys
rootprocid: ManageRegion
subprocid: ReprojectAncillaryRegionProjSys
author: thomasg
excerpt: Reproject ancillary region to predefined projsys
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
      "processid": "ReprojectAncillaryRegionProjSys",
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
        "layerid": "*",
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

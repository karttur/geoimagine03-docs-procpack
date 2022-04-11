---
layout: subprocess
categories: subprocess
title: OrganizeProjSysData
processurl: subprocid-OrganizeProjSysData
rootprocid: projsys
subprocid: OrganizeProjSysData
author: thomasg
excerpt: Projection system data import
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
      "processid": "OrganizeProjSysData",
      "parameters": {
        "importcode": "tif",
        "epsg": "4326",
        "orgid": "",
        "dsname": "",
        "dsversion": "0",
        "accessdate": "",
        "regionid": "",
        "regioncat": "",
        "dataurl": "",
        "metaurl": "",
        "title": "",
        "label": "",
        "copyright": "unknown",
        "replacestr": "",
        "replacetag": "",
        "tolerance": "0",
        "angletolerance": "0",
        "quadrangle": "False",
        "checkfixvalidity": "True",
        "ogr2ogr": "True",
        "cmdpath": "None",
        "wrapdateline": "False",
        "fieldNameDstL": "*",
        "attribFilter": ""
      },
      "srcpath": {
        "volume": "",
        "hdr": "",
        "dat": ""
      },
      "srcraw": [
        {
          "user_def_1": {
            "cellnull": "2222.2",
            "datadir": "",
            "datafile": "",
            "datalayer": "",
            "label": "Label for import data set",
            "title": ""
          }
        },
        {
          "user_def..n": {
            "cellnull": "2222.2",
            "datadir": "",
            "datafile": "",
            "datalayer": "",
            "label": "Label for import data set",
            "title": ""
          }
        }
      ],
      "dstcomp": [
        {
          "user_def_1": {
            "cellnull": "",
            "celltype": "",
            "content": "",
            "dataunit": "",
            "layerid": "*",
            "masked": "N",
            "measure": "N",
            "offsetadd": "0",
            "prefix": "",
            "product": "",
            "scalefac": "1",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "cellnull": "",
            "celltype": "",
            "content": "",
            "dataunit": "",
            "layerid": "*",
            "masked": "N",
            "measure": "N",
            "offsetadd": "0",
            "prefix": "",
            "product": "",
            "scalefac": "1",
            "source": "",
            "suffix": ""
          }
        }
      ],
      "dstpath": {
        "volume": "",
        "hdr": "shp",
        "dat": ""
      }
    }
  ]
}
```

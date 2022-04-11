---
layout: subprocess
categories: subprocess
title: OrganizeAncillary
processurl: subprocid-OrganizeAncillary
rootprocid: Ancillary
subprocid: OrganizeAncillary
author: thomasg
excerpt: Organize ancillary data
date: 2022-04-11
modified: 2022-04-11
comments: true
share: true
---

#### Complete json command structure (overriding defaults)
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
      "processid": "OrganizeAncillary",
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
#### Required json command structure (accepting all defaults)
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
      "processid": "OrganizeAncillary",
      "parameters": {
        "importcode": "tif",
        "orgid": "",
        "dsname": "",
        "regionid": "",
        "regioncat": ""
      },
      "srcpath": {
        "volume": "",
        "hdr": ""
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
        "volume": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | importcode | text | True | tif |
| process | parameters | epsg | integer | False | 4326 |
| process | parameters | orgid | text | True | --- |
| process | parameters | dsname | text | True | --- |
| process | parameters | dsversion | text | False | 0 |
| process | parameters | accessdate | text | False | --- |
| process | parameters | regionid | text | True | --- |
| process | parameters | regioncat | text | True | --- |
| process | parameters | dataurl | text | False | --- |
| process | parameters | metaurl | text | False | --- |
| process | parameters | title | text | False | --- |
| process | parameters | label | text | False | --- |
| process | parameters | copyright | text | False | unknown |
| process | parameters | replacestr | text | False | --- |
| process | parameters | replacetag | text | False | --- |
| process | parameters | tolerance | float | False | 0 |
| process | parameters | angletolerance | float | False | 0 |
| process | parameters | quadrangle | bool | False | False |
| process | parameters | checkfixvalidity | bool | False | True |
| process | parameters | ogr2ogr | bool | False | True |
| process | parameters | cmdpath | text | False | None |
| process | parameters | wrapdateline | bool | False | False |
| process | parameters | fieldNameDstL | text | False | * |
| process | parameters | attribFilter | text | False | --- |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | True | --- |
| process | srcpath | dat | text | False | --- |
| process | srcraw | * | element | True | * |
| process | dstcomp | * | element | True | * |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | shp |
| process | dstpath | dat | text | False | --- |

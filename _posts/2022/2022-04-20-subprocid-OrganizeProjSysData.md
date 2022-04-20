---
layout: subprocess
categories: subprocess
title: OrganizeProjSysData
processurl: subprocid-OrganizeProjSysData
rootprocid: projsys
subprocid: OrganizeProjSysData
author: thomasg
excerpt: Projection system data import
date: 2022-04-20
modified: 2022-04-20
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
      "processid": "OrganizeProjSysData",
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

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | importcode | Import code that identifies whith subroutine to use for import |
| process | parameters | epsg | EPSG 4-integer code of projection for dataset to import |
| process | parameters | orgid | Organisation id for dataset |
| process | parameters | dsname | Name of dataset to import |
| process | parameters | dsversion | Dataset version (if applicable) |
| process | parameters | accessdate | Date of accessing dataset (if left blank todays date will be recorded) |
| process | parameters | regionid | Default region id of the dataset |
| process | parameters | regioncat | Region category of the dataset |
| process | parameters | dataurl | url for source dataset |
| process | parameters | metaurl | url for source metadata |
| process | parameters | title | Source dataset title |
| process | parameters | label | Source dataset label |
| process | parameters | copyright | Source dataset copyright |
| process | parameters | replacestr | String to replace in multi-layered source datasets |
| process | parameters | replacetag | Tag identifying replacement identifying |
| process | parameters | tolerance | tolerance for simplifying vectors using distance |
| process | parameters | angletolerance | tolerance for simplifying vectors using angles |
| process | parameters | quadrangle | simplify vector polytgon to quadrangle |
| process | parameters | checkfixvalidity | check and fix validty of simplifed vector before saving |
| process | parameters | ogr2ogr | use ogr2ogr for importing vector, otehrwise use python scripting |
| process | parameters | cmdpath | path to gdal/ogr executable |
| process | parameters | wrapdateline | Wrap dateline for geographic data |
| process | parameters | fieldNameDstL | Comma separated name(s) of vector field names to copy |
| process | parameters | attribFilter | Attribute filter to apply for feature copying |
| process | srcpath | volume | Volume, disk or path containg the source data |
| process | srcpath | hdr | Header or header+data file extension |
| process | srcpath | dat | Data file extension for datasets with separate header + data file |
| process | srcraw | * | link for srcraw composition |
| process | dstcomp | * | link for destination composition |
| process | dstpath | volume | Volume, disk or path for saving the destination data |
| process | dstpath | hdr | Header or header+data file extension (default = shp) |
| process | dstpath | dat | Data file extension for datasets with separate header + data file |

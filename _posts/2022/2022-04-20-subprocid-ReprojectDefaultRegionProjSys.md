---
layout: subprocess
categories: subprocess
title: ReprojectDefaultRegionProjSys
processurl: subprocid-ReprojectDefaultRegionProjSys
rootprocid: ManageRegion
subprocid: ReprojectDefaultRegionProjSys
author: thomasg
excerpt: Reproject default region to predefined projsys
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
      "processid": "ReprojectDefaultRegionProjSys",
      "parameters": {
        "src_defregid": ""
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
        "volume": ""
      },
      "dstcopy": {
        "layerid": "*",
        "srccomp": "*"
      },
      "dstpath": {
        "volume": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | version | text | False | 1.3 |
| process | parameters | asscript | boolean | False | False |
| process | parameters | src_defregid | text | True | --- |
| process | parameters | checkfixvalidity | bool | False | True |
| process | parameters | ogr2ogr | bool | False | True |
| process | parameters | cmdpath | text | False | None |
| process | parameters | clipdst | boolean | False | True |
| process | parameters | tr_xres | real | False | 0 |
| process | parameters | tr_yres | real | False | 0 |
| process | parameters | resample | text | False | near |
| process | parameters | celltype | text | False | auto |
| process | parameters | errorthreshold | real | False | 0 |
| process | srccomp | * | element | True | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcopy | cellnull | integer | False | 0 |
| process | dstcopy | celltype | text | False | vector |
| process | dstcopy | dataunit | text | False | boundary |
| process | dstcopy | layerid | text | True | * |
| process | dstcopy | masked | text | False | N |
| process | dstcopy | measure | text | False | N |
| process | dstcopy | offsetadd | integer | False | 0 |
| process | dstcopy | scalefac | real | False | 1 |
| process | dstcopy | srccomp | text | True | * |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | version | to be completed |
| process | parameters | asscript | to be completed |
| process | parameters | src_defregid | The default region id of the source region to tile must be given |
| process | parameters | checkfixvalidity | check and fix validty of simplifed vector before saving |
| process | parameters | ogr2ogr | use ogr2ogr for importing vector, otehrwise use python scripting |
| process | parameters | cmdpath | path to gdal/ogr executable |
| process | parameters | clipdst | to be completed |
| process | parameters | tr_xres | to be completed |
| process | parameters | tr_yres | to be completed |
| process | parameters | resample | to be completed |
| process | parameters | celltype | to be completed |
| process | parameters | errorthreshold | error threshold for transformer (in pixels) 0 = auto |
| process | srccomp | * | link for source composition |
| process | srcpath | volume | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | dat | to be completed |
| process | dstcopy | cellnull | Regions do not have cellnull |
| process | dstcopy | celltype | All regions are vectors |
| process | dstcopy | dataunit | Regions are always of dataunit polygon |
| process | dstcopy | layerid | unknown hint |
| process | dstcopy | masked | All regions are unmasked |
| process | dstcopy | measure | All regions are of type Nominal |
| process | dstcopy | offsetadd | Regions have no offsetadd (=zero) |
| process | dstcopy | scalefac | Regions have no scalefac (=unity) |
| process | dstcopy | srccomp | unknown hint |
| process | dstpath | volume | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | dat | to be completed |

---
layout: subprocess
categories: subprocess
title: DefaultRegionFromVector
processurl: subprocid-DefaultRegionFromVector
rootprocid: ManageRegion
subprocid: DefaultRegionFromVector
author: thomasg
excerpt: Define default region from vector data set
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
      "processid": "DefaultRegionFromVector",
      "parameters": {
        "vector_db_id": "ISO_A3",
        "vector_db_name": "NAME",
        "vector_db_category": "",
        "vector_db_parentid": "PARENTID",
        "vector_db_parentcat": "PARENTCAT",
        "vector_db_stratum": "STRATUM",
        "vector_db_title": "TITLE",
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
        "volume": ""
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
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | vector_db_id | text | True | ISO_A3 |
| process | parameters | vector_db_name | text | True | NAME |
| process | parameters | vector_db_category | text | True | --- |
| process | parameters | vector_db_parentid | text | True | PARENTID |
| process | parameters | vector_db_parentcat | text | True | PARENTCAT |
| process | parameters | vector_db_stratum | text | True | STRATUM |
| process | parameters | vector_db_title | text | True | TITLE |
| process | parameters | vector_db_label | text | False | LABEL |
| process | parameters | version | text | True | 1.0 |
| process | srccomp | * | element | True | * |
| process | srccomp | element | text | False | * |
| process | srccomp | parent | text | False | process |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | shp |
| process | srcpath | dat | text | False | na |
| process | dstcopy | layerid | text | True | * |
| process | dstcopy | srccomp | text | True | * |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | True | shp |
| process | dstpath | dat | text | True | na |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | vector_db_id | Column in source vector db that defines default region id |
| process | parameters | vector_db_name | Column in source vector db that defines default region name |
| process | parameters | vector_db_category | Column in source vector db that defines default region category |
| process | parameters | vector_db_parentid | Column in source vector db that defines default region parent id |
| process | parameters | vector_db_parentcat | Column in source vector db that defines default region parent category |
| process | parameters | vector_db_stratum | Column in source vector db that defines default region pstratum |
| process | parameters | vector_db_title | Column in source vector db that defines default region title |
| process | parameters | vector_db_label | Column in source vector db that defines default region label |
| process | parameters | version | Default region version |
| process | srccomp | * | Hierarchical pointer |
| process | srccomp | element | Default hierarchical child name |
| process | srccomp | parent | Hierarchical object parent (for internal use) |
| process | srcpath | volume | Volume or disk |
| process | srcpath | hdr | Source vector data format |
| process | srcpath | dat | Data file extension for datasets with separate header + data file |
| process | dstcopy | layerid | unknown hint |
| process | dstcopy | srccomp | unknown hint |
| process | dstpath | volume | Volume or disk |
| process | dstpath | hdr | Header or header+data file extension |
| process | dstpath | dat | Data file extension for datasets with separate header + data file |

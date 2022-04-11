---
layout: subprocess
categories: subprocess
title: DefaultRegionFromVector
processurl: subprocid-DefaultRegionFromVector
rootprocid: ManageRegion
subprocid: DefaultRegionFromVector
author: thomasg
excerpt: Define default region from vector data set
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

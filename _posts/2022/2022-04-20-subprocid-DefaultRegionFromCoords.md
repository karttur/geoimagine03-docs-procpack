---
layout: subprocess
categories: subprocess
title: DefaultRegionFromCoords
processurl: subprocid-DefaultRegionFromCoords
rootprocid: ManageRegion
subprocid: DefaultRegionFromCoords
author: thomasg
excerpt: Define default region for public use from corner coordinates
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
      "processid": "DefaultRegionFromCoords",
      "parameters": {
        "regionid": "",
        "regionname": "",
        "regioncat": "",
        "parentid": "",
        "parentcat": "",
        "stratum": "0",
        "minx": "0",
        "maxx": "0",
        "miny": "0",
        "maxy": "0",
        "epsg": "4326",
        "version": "1.0",
        "title": "Title",
        "label": "Label"
      },
      "dstcomp": [
        {
          "user_def_1": {
            "cellnull": "0",
            "celltype": "vector",
            "content": "roi",
            "dataunit": "boundary",
            "layerid": "defreg",
            "masked": "N",
            "measure": "N",
            "offsetadd": "0",
            "prefix": "defreg",
            "product": "pubroi",
            "scalefac": "1",
            "source": "karttur",
            "suffix": "v010"
          }
        },
        {
          "user_def..n": {
            "cellnull": "0",
            "celltype": "vector",
            "content": "roi",
            "dataunit": "boundary",
            "layerid": "defreg",
            "masked": "N",
            "measure": "N",
            "offsetadd": "0",
            "prefix": "defreg",
            "product": "pubroi",
            "scalefac": "1",
            "source": "karttur",
            "suffix": "v010"
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
      "processid": "DefaultRegionFromCoords",
      "parameters": {
        "regionid": "",
        "regionname": "",
        "regioncat": "",
        "parentid": "",
        "parentcat": "",
        "stratum": "0",
        "minx": "0",
        "maxx": "0",
        "miny": "0",
        "maxy": "0"
      },
      "dstcomp": [
        {
          "user_def_1": {}
        },
        {
          "user_def..n": {}
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
| process | parameters | regionid | text | True | --- |
| process | parameters | regionname | text | True | --- |
| process | parameters | regioncat | text | True | --- |
| process | parameters | parentid | text | True | --- |
| process | parameters | parentcat | text | True | --- |
| process | parameters | stratum | integer | True | 0 |
| process | parameters | minx | float | True | 0 |
| process | parameters | maxx | float | True | 0 |
| process | parameters | miny | float | True | 0 |
| process | parameters | maxy | float | True | 0 |
| process | parameters | epsg | integer | False | 4326 |
| process | parameters | version | text | False | 1.0 |
| process | parameters | title | text | False | Title |
| process | parameters | label | text | False | Label |
| process | dstcomp | * | element | False | * |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | shp |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | regionid | Set an id for the default region |
| process | parameters | regionname | Default region name (must be unique) |
| process | parameters | regioncat | Default region category |
| process | parameters | parentid | Default region parent regionid |
| process | parameters | parentcat | Default region parent region category |
| process | parameters | stratum | Stratum for region access |
| process | parameters | minx | x-coord or longitude minimum |
| process | parameters | maxx | x-coord or longitude maximum |
| process | parameters | miny | y-coord or latitude minimum |
| process | parameters | maxy | y-coord or latitude maximum |
| process | parameters | epsg | EPSG code for region |
| process | parameters | version | Region version |
| process | parameters | title | Region title |
| process | parameters | label | Region label |
| process | dstcomp | * | 1:1 link for destination composition |
| process | dstpath | volume | Volume, disk or path for saving the destination data |
| process | dstpath | hdr | Header or header+data file extension (default = shp) |
| process | dstpath | dat | Data file extension for datasets with separate header + data file |

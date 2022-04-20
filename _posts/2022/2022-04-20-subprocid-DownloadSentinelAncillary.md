---
layout: subprocess
categories: subprocess
title: DownloadSentinelAncillary
processurl: subprocid-DownloadSentinelAncillary
rootprocid: SentinelProcess
subprocid: DownloadSentinelAncillary
author: thomasg
excerpt: Download Sentinel granule meta data
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
      "processid": "DownloadSentinelAncillary",
      "parameters": {
        "tablesearchid": "searchid",
        "granuleoverlap": "0.1",
        "orbitdirection": "B",
        "platformname": "Sentinel-2",
        "prodtype": "S2MSI1C",
        "cloudmax": "30",
        "startdate": "20140401",
        "enddate": "20180821",
        "startdoy": "1",
        "enddoy": "365"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "vector",
            "layerid": "vector",
            "prefix": "vector",
            "product": "",
            "source": "*",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "vector",
            "layerid": "vector",
            "prefix": "vector",
            "product": "",
            "source": "*",
            "suffix": ""
          }
        }
      ],
      "srcpath": {
        "volume": "",
        "hdr": "shp",
        "dat": "shp"
      },
      "dstpath": {
        "volume": "",
        "hdr": "zip",
        "dat": "zip"
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
      "processid": "DownloadSentinelAncillary",
      "parameters": {
        "orbitdirection": "B",
        "platformname": "Sentinel-2",
        "prodtype": "S2MSI1C",
        "cloudmax": "30",
        "startdate": "20140401",
        "enddate": "20180821"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "vector",
            "layerid": "vector",
            "prefix": "vector",
            "product": "",
            "source": "*",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "vector",
            "layerid": "vector",
            "prefix": "vector",
            "product": "",
            "source": "*",
            "suffix": ""
          }
        }
      ],
      "srcpath": {
        "volume": ""
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
| process | parameters | tablesearchid | text | False | searchid |
| process | parameters | granuleoverlap | real | False | 0.1 |
| process | parameters | orbitdirection | text | True | B |
| process | parameters | platformname | text | True | Sentinel-2 |
| process | parameters | prodtype | text | True | S2MSI1C |
| process | parameters | cloudmax | integer | True | 30 |
| process | parameters | startdate | date | True | 20140401 |
| process | parameters | enddate | date | True | 20180821 |
| process | parameters | startdoy | integer | False | 1 |
| process | parameters | enddoy | integer | False | 365 |
| process | srccomp | * | element | True | * |
| process | srccomp | element | text | False | * |
| process | srccomp | parent | text | False | process |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | shp |
| process | srcpath | dat | text | False | shp |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | zip |
| process | dstpath | dat | text | False | zip |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | tablesearchid | to be completed |
| process | parameters | granuleoverlap | to be completed |
| process | parameters | orbitdirection | to be completed |
| process | parameters | platformname | to be completed |
| process | parameters | prodtype | to be completed |
| process | parameters | cloudmax | to be completed |
| process | parameters | startdate | to be completed |
| process | parameters | enddate | to be completed |
| process | parameters | startdoy | to be completed |
| process | parameters | enddoy | to be completed |
| process | srccomp | * | to be completed |
| process | srccomp | element | to be completed |
| process | srccomp | parent | to be completed |
| process | srcpath | volume | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | dat | to be completed |
| process | dstpath | volume | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | dat | to be completed |

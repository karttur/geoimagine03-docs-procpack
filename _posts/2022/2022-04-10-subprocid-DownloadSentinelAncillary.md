---
layout: subprocess
categories: subprocess
title: DownloadSentinelAncillary
processurl: subprocid-DownloadSentinelAncillary
rootprocid: SentinelProcess
subprocid: DownloadSentinelAncillary
author: thomasg
excerpt: Download Sentinel granule meta data
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

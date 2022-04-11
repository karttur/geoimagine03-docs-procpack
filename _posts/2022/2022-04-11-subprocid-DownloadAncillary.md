---
layout: subprocess
categories: subprocess
title: DownloadAncillary
processurl: subprocid-DownloadAncillary
rootprocid: Ancillary
subprocid: DownloadAncillary
author: thomasg
excerpt: Download ancillary data
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
      "processid": "DownloadAncillary",
      "parameters": {
        "downloadcode": "urlstring",
        "path": "",
        "datadir": ""
      },
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
      "processid": "DownloadAncillary",
      "parameters": {
        "downloadcode": "urlstring",
        "path": "",
        "datadir": ""
      },
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
| process | parameters | downloadcode | text | True | urlstring |
| process | parameters | path | text | True | --- |
| process | parameters | datadir | text | True | --- |
| process | srcpath | volume | text | True | --- |
| process | dstpath | volume | text | True | --- |

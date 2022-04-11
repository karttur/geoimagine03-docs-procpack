---
layout: subprocess
categories: subprocess
title: FtpAncillary
processurl: subprocid-FtpAncillary
rootprocid: Ancillary
subprocid: FtpAncillary
author: thomasg
excerpt: FTP access and Download ancillary data
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
      "processid": "FtpAncillary",
      "parameters": {
        "downloadcode": "urlstring",
        "path": "",
        "datadir": "",
        "host": "",
        "port": "21",
        "encryptation": "normal",
        "logontype": "normal",
        "user": "anonymous",
        "password": "none"
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
      "processid": "FtpAncillary",
      "parameters": {
        "downloadcode": "urlstring",
        "path": "",
        "datadir": "",
        "host": "",
        "user": "anonymous",
        "password": "none"
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
| process | parameters | host | text | True | --- |
| process | parameters | port | text | False | 21 |
| process | parameters | encryptation | text | False | normal |
| process | parameters | logontype | text | False | normal |
| process | parameters | user | text | True | anonymous |
| process | parameters | password | text | True | none |
| process | srcpath | volume | text | True | --- |
| process | dstpath | volume | text | True | --- |

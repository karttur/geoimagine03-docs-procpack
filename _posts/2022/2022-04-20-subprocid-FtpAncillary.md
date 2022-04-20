---
layout: subprocess
categories: subprocess
title: FtpAncillary
processurl: subprocid-FtpAncillary
rootprocid: Ancillary
subprocid: FtpAncillary
author: thomasg
excerpt: FTP access and Download ancillary data
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

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | downloadcode | Import code that identifies which subroutine to use for import |
| process | parameters | path | path to download regardless of what kind |
| process | parameters | datadir | path under dstpath where to save file |
| process | parameters | host | ftpserver to connect to |
| process | parameters | port | port for connecting |
| process | parameters | encryptation | Encryptation, if required |
| process | parameters | logontype | Logon type, if required |
| process | parameters | user | Registered user for FTP server |
| process | parameters | password | User password for FTP server |
| process | srcpath | volume | Volume, disk or path for saving the destination data |
| process | dstpath | volume | Volume, disk or path for saving the destination data |

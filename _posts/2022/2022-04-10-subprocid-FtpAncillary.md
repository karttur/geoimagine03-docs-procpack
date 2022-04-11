---
layout: subprocess
categories: subprocess
title: FtpAncillary
processurl: subprocid-FtpAncillary
rootprocid: Ancillary
subprocid: FtpAncillary
author: thomasg
excerpt: FTP access and Download ancillary data
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

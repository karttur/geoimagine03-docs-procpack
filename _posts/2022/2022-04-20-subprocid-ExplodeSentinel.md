---
layout: subprocess
categories: subprocess
title: ExplodeSentinel
processurl: subprocid-ExplodeSentinel
rootprocid: SentinelProcess
subprocid: ExplodeSentinel
author: thomasg
excerpt: Explode Sentinel tiles
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
      "processid": "ExplodeSentinel",
      "parameters": {
        "granuleoverlap": "0.1",
        "orbitdirection": "B",
        "platformname": "Sentinel-2",
        "exploded": "N",
        "prodtype": "S2MSI1C",
        "cloudmax": "0",
        "setcloudmask": "True",
        "setdetfoomask": "True",
        "setnodatamask": "True",
        "setdefectask": "True",
        "setsaturamask": "True",
        "settecquamask": "False",
        "set0tonull": "True"
      },
      "srcpath": {
        "dat": "zip",
        "hdr": "zip",
        "volume": ""
      },
      "dstpath": {
        "dat": "tif",
        "hdr": "tif",
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
      "processid": "ExplodeSentinel",
      "parameters": {
        "platformname": "Sentinel-2",
        "prodtype": "S2MSI1C"
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
| process | parameters | granuleoverlap | float | False | 0.1 |
| process | parameters | orbitdirection | text | False | B |
| process | parameters | platformname | text | True | Sentinel-2 |
| process | parameters | exploded | text | False | N |
| process | parameters | prodtype | text | True | S2MSI1C |
| process | parameters | cloudmax | integer | False | 0 |
| process | parameters | setcloudmask | boolean | False | True |
| process | parameters | setdetfoomask | boolean | False | True |
| process | parameters | setnodatamask | boolean | False | True |
| process | parameters | setdefectask | boolean | False | True |
| process | parameters | setsaturamask | boolean | False | True |
| process | parameters | settecquamask | boolean | False | False |
| process | parameters | set0tonull | boolean | False | True |
| process | srcpath | dat | text | False | zip |
| process | srcpath | hdr | text | False | zip |
| process | srcpath | volume | text | True | --- |
| process | dstpath | dat | text | False | tif |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | granuleoverlap | to be completed |
| process | parameters | orbitdirection | to be completed |
| process | parameters | platformname | to be completed |
| process | parameters | exploded | to be completed |
| process | parameters | prodtype | to be completed |
| process | parameters | cloudmax | to be completed |
| process | parameters | setcloudmask | to be completed |
| process | parameters | setdetfoomask | to be completed |
| process | parameters | setnodatamask | to be completed |
| process | parameters | setdefectask | to be completed |
| process | parameters | setsaturamask | to be completed |
| process | parameters | settecquamask | to be completed |
| process | parameters | set0tonull | to be completed |
| process | srcpath | dat | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | volume | to be completed |
| process | dstpath | dat | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | volume | to be completed |

---
layout: subprocess
categories: subprocess
title: ExtractModisPolarHdf
processurl: subprocid-ExtractModisPolarHdf
rootprocid: ModisPolar
subprocid: ExtractModisPolarHdf
author: thomasg
excerpt: Extracts the content of modis NSIDC data>
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
      "processid": "ExtractModisPolarHdf",
      "parameters": {
        "asscript": "True",
        "product": "MYD29E1D",
        "version": "006"
      },
      "srcpath": {
        "dat": "",
        "hdr": "hdf",
        "volume": ""
      },
      "dstpath": {
        "dat": "",
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
      "processid": "ExtractModisPolarHdf",
      "parameters": {
        "product": "MYD29E1D",
        "version": "006"
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
| process | parameters | asscript | boolean | False | True |
| process | parameters | product | text | True | MYD29E1D |
| process | parameters | version | text | True | 006 |
| process | srcpath | dat | text | False | --- |
| process | srcpath | hdr | text | False | hdf |
| process | srcpath | volume | text | True | --- |
| process | dstpath | dat | text | False | --- |
| process | dstpath | hdr | text | False | tif |
| process | dstpath | volume | text | True | --- |

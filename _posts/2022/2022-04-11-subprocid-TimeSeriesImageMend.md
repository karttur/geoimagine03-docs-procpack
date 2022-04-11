---
layout: subprocess
categories: subprocess
title: TimeSeriesImageMend
processurl: subprocid-TimeSeriesImageMend
rootprocid: TimeSeries
subprocid: TimeSeriesImageMend
author: thomasg
excerpt: Mend image timeseries data
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
      "processid": "TimeSeriesImageMend",
      "parameters": {
        "copycomp": "1to1",
        "version": "1.3",
        "method": "interpolate",
        "validfraction": "0.5"
      },
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        }
      ],
      "srcpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      },
      "dstcomp": [
        {
          "user_def_1": {
            "content": "src",
            "layerid": "*",
            "prefix": "*",
            "product": "src",
            "source": "src",
            "suffix": "*"
          }
        },
        {
          "user_def..n": {
            "content": "src",
            "layerid": "*",
            "prefix": "*",
            "product": "src",
            "source": "src",
            "suffix": "*"
          }
        }
      ],
      "dstpath": {
        "volume": "",
        "hdr": "tif",
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
      "processid": "TimeSeriesImageMend",
      "parameters": {},
      "srccomp": [
        {
          "user_def_1": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "content": "",
            "layerid": "*",
            "prefix": "",
            "product": "",
            "source": "",
            "suffix": ""
          }
        }
      ],
      "srcpath": {
        "volume": "",
        "hdr": "tif"
      },
      "dstcomp": [
        {
          "user_def_1": {
            "content": "src",
            "layerid": "*",
            "prefix": "*",
            "product": "src",
            "source": "src",
            "suffix": "*"
          }
        },
        {
          "user_def..n": {
            "content": "src",
            "layerid": "*",
            "prefix": "*",
            "product": "src",
            "source": "src",
            "suffix": "*"
          }
        }
      ],
      "dstpath": {
        "volume": "",
        "hdr": "tif"
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | copycomp | text | False | 1to1 |
| process | parameters | version | text | False | 1.3 |
| process | parameters | method | text | False | interpolate |
| process | parameters | validfraction | real | False | 0.5 |
| process | srccomp | * | element | True | * |
| process | srccomp | element | text | False | * |
| process | srccomp | parent | text | False | process |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | True | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcomp | * | element | True | * |
| process | dstcomp | element | text | False | * |
| process | dstcomp | parent | text | False | process |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | True | tif |
| process | dstpath | dat | text | False | --- |

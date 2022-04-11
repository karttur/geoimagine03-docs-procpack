---
layout: subprocess
categories: subprocess
title: Periodicity
processurl: subprocid-Periodicity
rootprocid: Periodicity
subprocid: Periodicity
author: thomasg
excerpt: Period settings
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
      "processid": "Periodicity",
      "srcperiod": {
        "addons": "0",
        "maxdaysaddons": "0",
        "timestep": "NA"
      },
      "dstperiod": {
        "timestep": "NA"
      },
      "period": {
        "addons": "0",
        "averagets": "False",
        "endday": "31",
        "endmonth": "12",
        "endyear": "2100",
        "maxdaysaddons": "0",
        "seasonalts": "False",
        "seasonendday": "31",
        "seasonendmonth": "12",
        "seasonstartday": "1",
        "seasonstartmonth": "1",
        "startday": "1",
        "startmonth": "1",
        "startyear": "1900",
        "timestep": "static"
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
      "processid": "Periodicity",
      "srcperiod": {},
      "dstperiod": {},
      "period": {}
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | srcperiod | addons | integer | False | 0 |
| process | srcperiod | maxdaysaddons | integer | False | 0 |
| process | srcperiod | timestep | text | False | NA |
| process | dstperiod | timestep | text | False | NA |
| process | period | addons | integer | False | 0 |
| process | period | averagets | boolean | False | False |
| process | period | endday | integer | False | 31 |
| process | period | endmonth | integer | False | 12 |
| process | period | endyear | integer | False | 2100 |
| process | period | maxdaysaddons | integer | False | 0 |
| process | period | seasonalts | boolean | False | False |
| process | period | seasonendday | integer | False | 31 |
| process | period | seasonendmonth | integer | False | 12 |
| process | period | seasonstartday | integer | False | 1 |
| process | period | seasonstartmonth | integer | False | 1 |
| process | period | startday | integer | False | 1 |
| process | period | startmonth | integer | False | 1 |
| process | period | startyear | integer | False | 1900 |
| process | period | timestep | text | False | static |

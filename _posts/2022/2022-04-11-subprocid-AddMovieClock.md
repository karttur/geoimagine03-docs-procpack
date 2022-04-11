---
layout: subprocess
categories: subprocess
title: AddMovieClock
processurl: subprocid-AddMovieClock
rootprocid: LayoutProc
subprocid: AddMovieClock
author: thomasg
excerpt: Add movieclock layout
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
      "processid": "AddMovieClock",
      "parameters": {
        "name": "",
        "tlmargin": "{5,5,5,5}",
        "clmargin": "{5,5,5,5}",
        "position": "ll",
        "bgcolor": "black",
        "tlborder": "2",
        "clborder": "6",
        "tlbordercolor": "beige",
        "clbordercolor": "beige",
        "clcolor": "blue",
        "tlheight": "10",
        "tlticks": "1",
        "tltickwidth": "2",
        "tickcolor": "beige",
        "boettcolor": "silver",
        "textatclock": "False",
        "tlcolor": "purple",
        "clradius": "50",
        "clhandcolor": "purple",
        "clframecolor": "black",
        "fontsize": "24",
        "fontcolor": "grey",
        "fontbackground": "black",
        "rotate": "0",
        "font": "Arial",
        "textinvideo": "False",
        "transparent": "black"
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
      "processid": "AddMovieClock",
      "parameters": {
        "name": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | name | text | True | --- |
| process | parameters | tlmargin | string | False | {5,5,5,5} |
| process | parameters | clmargin | string | False | {5,5,5,5} |
| process | parameters | position | text | False | ll |
| process | parameters | bgcolor | text | False | black |
| process | parameters | tlborder | integer | False | 2 |
| process | parameters | clborder | integer | False | 6 |
| process | parameters | tlbordercolor | text | False | beige |
| process | parameters | clbordercolor | text | False | beige |
| process | parameters | clcolor | text | False | blue |
| process | parameters | tlheight | integer | False | 10 |
| process | parameters | tlticks | integer | False | 1 |
| process | parameters | tltickwidth | integer | False | 2 |
| process | parameters | tickcolor | text | False | beige |
| process | parameters | boettcolor | text | False | silver |
| process | parameters | textatclock | bool | False | False |
| process | parameters | tlcolor | text | False | purple |
| process | parameters | clradius | integer | False | 50 |
| process | parameters | clhandcolor | text | False | purple |
| process | parameters | clframecolor | text | False | black |
| process | parameters | fontsize | integer | False | 24 |
| process | parameters | fontcolor | text | False | grey |
| process | parameters | fontbackground | text | False | black |
| process | parameters | rotate | integer | False | 0 |
| process | parameters | font | text | False | Arial |
| process | parameters | textinvideo | bool | False | False |
| process | parameters | transparent | text | False | black |

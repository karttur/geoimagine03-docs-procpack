---
layout: subprocess
categories: subprocess
title: CreateLegend
processurl: subprocid-CreateLegend
rootprocid: LayoutProc
subprocid: CreateLegend
author: thomasg
excerpt: Create legend for raster layer
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
      "processid": "CreateLegend",
      "parameters": {
        "palmax": "250",
        "palmin": "0",
        "two51": "False",
        "two52": "False",
        "two53": "False",
        "two54": "False",
        "two55": "False",
        "height": "500",
        "width": "100",
        "soloheight": "70",
        "pngwidth": "300",
        "pngheight": "300",
        "measure": "A",
        "buffer": "{10,10,10,10}",
        "margin": "{10,5,10,5}",
        "textpadding": "{10,5,10,5}",
        "framecolor": "254",
        "framefill": "black",
        "framestrokewidth": "1.0",
        "label": "True",
        "fontcolor": "black",
        "font": "Verdana",
        "fontsize": "12",
        "fonteffect": "",
        "titlefontcolor": "black",
        "titlefont": "Verdana",
        "titlefontsize": "16",
        "titlefonteffect": "",
        "sticklen": "10",
        "compresslabels": "False",
        "separatebuffer": "{5,5,5,5}",
        "precision": "0",
        "columnhead": "",
        "columns": "1",
        "matrix": "False",
        "columntext": "",
        "rowtext": "",
        "rowhead": ""
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
      ]
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
      "processid": "CreateLegend",
      "parameters": {
        "columnhead": ""
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
      ]
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | palmax | integer | False | 250 |
| process | parameters | palmin | integer | False | 0 |
| process | parameters | two51 | boolean | False | False |
| process | parameters | two52 | boolean | False | False |
| process | parameters | two53 | boolean | False | False |
| process | parameters | two54 | boolean | False | False |
| process | parameters | two55 | boolean | False | False |
| process | parameters | height | integer | False | 500 |
| process | parameters | width | integer | False | 100 |
| process | parameters | soloheight | integer | False | 70 |
| process | parameters | pngwidth | integer | False | 300 |
| process | parameters | pngheight | integer | False | 300 |
| process | parameters | measure | text | False | A |
| process | parameters | buffer | string | False | {10,10,10,10} |
| process | parameters | margin | string | False | {10,5,10,5} |
| process | parameters | textpadding | string | False | {10,5,10,5} |
| process | parameters | framecolor | integer | False | 254 |
| process | parameters | framefill | text | False | black |
| process | parameters | framestrokewidth | real | False | 1.0 |
| process | parameters | label | bool | False | True |
| process | parameters | fontcolor | text | False | black |
| process | parameters | font | text | False | Verdana |
| process | parameters | fontsize | integer | False | 12 |
| process | parameters | fonteffect | text | False | --- |
| process | parameters | titlefontcolor | text | False | black |
| process | parameters | titlefont | text | False | Verdana |
| process | parameters | titlefontsize | integer | False | 16 |
| process | parameters | titlefonteffect | text | False | --- |
| process | parameters | sticklen | integer | False | 10 |
| process | parameters | compresslabels | boolean | False | False |
| process | parameters | separatebuffer | string | False | {5,5,5,5} |
| process | parameters | precision | text | False | 0 |
| process | parameters | columnhead | text | True | --- |
| process | parameters | columns | integer | False | 1 |
| process | parameters | matrix | bool | False | False |
| process | parameters | columntext | text | False | --- |
| process | parameters | rowtext | text | False | --- |
| process | parameters | rowhead | text | False | --- |
| process | srccomp | * | element | True | * |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | palmax | to be completed |
| process | parameters | palmin | to be completed |
| process | parameters | two51 | to be completed |
| process | parameters | two52 | to be completed |
| process | parameters | two53 | to be completed |
| process | parameters | two54 | to be completed |
| process | parameters | two55 | to be completed |
| process | parameters | height | to be completed |
| process | parameters | width | to be completed |
| process | parameters | soloheight | to be completed |
| process | parameters | pngwidth | to be completed |
| process | parameters | pngheight | to be completed |
| process | parameters | measure | to be completed |
| process | parameters | buffer | to be completed |
| process | parameters | margin | to be completed |
| process | parameters | textpadding | to be completed |
| process | parameters | framecolor | to be completed |
| process | parameters | framefill | to be completed |
| process | parameters | framestrokewidth | to be completed |
| process | parameters | label | to be completed |
| process | parameters | fontcolor | to be completed |
| process | parameters | font | to be completed |
| process | parameters | fontsize | to be completed |
| process | parameters | fonteffect | to be completed |
| process | parameters | titlefontcolor | to be completed |
| process | parameters | titlefont | to be completed |
| process | parameters | titlefontsize | to be completed |
| process | parameters | titlefonteffect | to be completed |
| process | parameters | sticklen | to be completed |
| process | parameters | compresslabels | to be completed |
| process | parameters | separatebuffer | to be completed |
| process | parameters | precision | to be completed |
| process | parameters | columnhead | to be completed |
| process | parameters | columns | to be completed |
| process | parameters | matrix | to be completed |
| process | parameters | columntext | to be completed |
| process | parameters | rowtext | to be completed |
| process | parameters | rowhead | to be completed |
| process | srccomp | * | link for source composition |

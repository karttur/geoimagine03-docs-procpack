---
layout: subprocess
categories: subprocess
title: ExportLegend
processurl: subprocid-ExportLegend
rootprocid: LayoutProc
subprocid: ExportLegend
author: thomasg
excerpt: Export legend for raster layer
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
      "processid": "ExportLegend",
      "parameters": {
        "palette": "",
        "legendnominal": "False",
        "legendbackground": "White",
        "legendopacity": "0",
        "legendpalmax": "250",
        "legendpalmin": "0",
        "legendtwo51": "False",
        "legendtwo52": "False",
        "legendtwo53": "False",
        "legendtwo54": "False",
        "legendtwo55": "False",
        "legendheight": "500",
        "legendwidth": "100",
        "legendsoloheight": "70",
        "legendpngwidth": "300",
        "legendpngheight": "300",
        "measure": "A",
        "legendbuffer": "10",
        "legendmargin": "10",
        "legendtextpadding": "10",
        "legendframecolor": "254",
        "legendframefill": "black",
        "legendframestrokewidth": "1.0",
        "legendlabel": "True",
        "legendfontcolor": "black",
        "legendfont": "Verdana",
        "legendfontsize": "12",
        "legendfonteffect": "",
        "legendtitlefontcolor": "black",
        "legendtitlefont": "Verdana",
        "legendtitlefontsize": "12",
        "legendtitlefonteffect": "",
        "legendsticklen": "10",
        "legendcompresslabels": "False",
        "legendseparatebuffer": "10",
        "legendcolumnhead": "",
        "legendcolumns": "1",
        "legendmatrix": "False",
        "legendcolumntext": "",
        "legendrowtext": "",
        "legendrowhead": "",
        "jpg": "0"
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
      "processid": "ExportLegend",
      "parameters": {
        "palette": ""
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
      "dstpath": {
        "volume": ""
      }
    }
  ]
}
```
#### List of parameters

| **parent** | **element** | **paramid** | **type** | **required** | **default** |
| process | parameters | palette | text | True | --- |
| process | parameters | legendnominal | boolean | False | False |
| process | parameters | legendbackground | text | False | White |
| process | parameters | legendopacity | integer | False | 0 |
| process | parameters | legendpalmax | integer | False | 250 |
| process | parameters | legendpalmin | integer | False | 0 |
| process | parameters | legendtwo51 | boolean | False | False |
| process | parameters | legendtwo52 | boolean | False | False |
| process | parameters | legendtwo53 | boolean | False | False |
| process | parameters | legendtwo54 | boolean | False | False |
| process | parameters | legendtwo55 | boolean | False | False |
| process | parameters | legendheight | integer | False | 500 |
| process | parameters | legendwidth | integer | False | 100 |
| process | parameters | legendsoloheight | integer | False | 70 |
| process | parameters | legendpngwidth | integer | False | 300 |
| process | parameters | legendpngheight | integer | False | 300 |
| process | parameters | measure | text | False | A |
| process | parameters | legendbuffer | integer | False | 10 |
| process | parameters | legendmargin | integer | False | 10 |
| process | parameters | legendtextpadding | integer | False | 10 |
| process | parameters | legendframecolor | integer | False | 254 |
| process | parameters | legendframefill | text | False | black |
| process | parameters | legendframestrokewidth | real | False | 1.0 |
| process | parameters | legendlabel | bool | False | True |
| process | parameters | legendfontcolor | text | False | black |
| process | parameters | legendfont | text | False | Verdana |
| process | parameters | legendfontsize | integer | False | 12 |
| process | parameters | legendfonteffect | text | False | --- |
| process | parameters | legendtitlefontcolor | text | False | black |
| process | parameters | legendtitlefont | text | False | Verdana |
| process | parameters | legendtitlefontsize | integer | False | 12 |
| process | parameters | legendtitlefonteffect | text | False | --- |
| process | parameters | legendsticklen | integer | False | 10 |
| process | parameters | legendcompresslabels | boolean | False | False |
| process | parameters | legendseparatebuffer | integer | False | 10 |
| process | parameters | legendcolumnhead | text | False | --- |
| process | parameters | legendcolumns | integer | False | 1 |
| process | parameters | legendmatrix | bool | False | False |
| process | parameters | legendcolumntext | text | False | --- |
| process | parameters | legendrowtext | text | False | --- |
| process | parameters | legendrowhead | text | False | --- |
| process | parameters | jpg | integer | False | 0 |
| process | srccomp | * | element | True | * |
| process | dstpath | volume | text | True | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | palette | to be completed |
| process | parameters | legendnominal | to be completed |
| process | parameters | legendbackground | to be completed |
| process | parameters | legendopacity | to be completed |
| process | parameters | legendpalmax | to be completed |
| process | parameters | legendpalmin | to be completed |
| process | parameters | legendtwo51 | to be completed |
| process | parameters | legendtwo52 | to be completed |
| process | parameters | legendtwo53 | to be completed |
| process | parameters | legendtwo54 | to be completed |
| process | parameters | legendtwo55 | to be completed |
| process | parameters | legendheight | to be completed |
| process | parameters | legendwidth | to be completed |
| process | parameters | legendsoloheight | to be completed |
| process | parameters | legendpngwidth | to be completed |
| process | parameters | legendpngheight | to be completed |
| process | parameters | measure | to be completed |
| process | parameters | legendbuffer | to be completed |
| process | parameters | legendmargin | to be completed |
| process | parameters | legendtextpadding | to be completed |
| process | parameters | legendframecolor | to be completed |
| process | parameters | legendframefill | to be completed |
| process | parameters | legendframestrokewidth | to be completed |
| process | parameters | legendlabel | to be completed |
| process | parameters | legendfontcolor | to be completed |
| process | parameters | legendfont | to be completed |
| process | parameters | legendfontsize | to be completed |
| process | parameters | legendfonteffect | to be completed |
| process | parameters | legendtitlefontcolor | to be completed |
| process | parameters | legendtitlefont | to be completed |
| process | parameters | legendtitlefontsize | to be completed |
| process | parameters | legendtitlefonteffect | to be completed |
| process | parameters | legendsticklen | to be completed |
| process | parameters | legendcompresslabels | to be completed |
| process | parameters | legendseparatebuffer | to be completed |
| process | parameters | legendcolumnhead | to be completed |
| process | parameters | legendcolumns | to be completed |
| process | parameters | legendmatrix | to be completed |
| process | parameters | legendcolumntext | to be completed |
| process | parameters | legendrowtext | to be completed |
| process | parameters | legendrowhead | to be completed |
| process | parameters | jpg | to be completed |
| process | srccomp | * | link for source composition |
| process | dstpath | volume | to be completed |

---
layout: subprocess
categories: subprocess
title: ExportTilesToByte
processurl: subprocid-ExportTilesToByte
rootprocid: Export
subprocid: ExportTilesToByte
author: thomasg
excerpt: Export tiles to byte binary
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
      "processid": "ExportTilesToByte",
      "parameters": {
        "overwritelayout": "False",
        "palette": "default",
        "minmax": "False",
        "srcmin": "0",
        "srcmax": "0",
        "zscore": "false",
        "globalmeantozero": "True",
        "globalmean": "0",
        "globalstd": "0",
        "zscorefac": "1",
        "dynamicmask": "False",
        "masknotnullin": "255",
        "vectoroverlay": "",
        "width": "0",
        "crop": "",
        "border": "0",
        "bordercolor": "black",
        "emboss": "",
        "embossdims": "0",
        "embossptsize": "0",
        "title": "",
        "titlesingleline": "True",
        "titlegravity": "North",
        "titlebackgroundcolor": "white",
        "titlefontcolor": "black",
        "titlefont": "Tahoma",
        "titlefontsize": "12",
        "detailcrop": "",
        "detailwidth": "0",
        "detailborder": "2",
        "detailbordercolor": "black",
        "detailtitle": "True",
        "detaillegend": "False",
        "detaillegendgravity": "East",
        "detaillegendsize": "100",
        "detaillegendbackground": "White",
        "jpg": "0",
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
        "legendrowhead": ""
      },
      "srccomp": [
        {
          "user_def_1": {
            "source": "",
            "product": "",
            "content": "",
            "layerid": "*",
            "prefix": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "source": "",
            "product": "",
            "content": "",
            "layerid": "*",
            "prefix": "",
            "suffix": ""
          }
        }
      ],
      "srcpath": {
        "volume": "",
        "hdr": "tif",
        "dat": ""
      },
      "dstcopy": {
        "srccomp": "*",
        "layerid": "copy",
        "prefix": "copy",
        "suffix": "copy"
      },
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
      "processid": "ExportTilesToByte",
      "parameters": {},
      "srccomp": [
        {
          "user_def_1": {
            "source": "",
            "product": "",
            "content": "",
            "layerid": "*",
            "prefix": "",
            "suffix": ""
          }
        },
        {
          "user_def..n": {
            "source": "",
            "product": "",
            "content": "",
            "layerid": "*",
            "prefix": "",
            "suffix": ""
          }
        }
      ],
      "srcpath": {
        "volume": "",
        "hdr": "tif"
      },
      "dstcopy": {
        "srccomp": "*"
      },
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
| process | parameters | overwritelayout | boolean | False | False |
| process | parameters | palette | text | False | default |
| process | parameters | minmax | boolean | False | False |
| process | parameters | srcmin | float | False | 0 |
| process | parameters | srcmax | float | False | 0 |
| process | parameters | zscore | boolean | False | false |
| process | parameters | globalmeantozero | boolean | False | True |
| process | parameters | globalmean | float | False | 0 |
| process | parameters | globalstd | float | False | 0 |
| process | parameters | zscorefac | float | False | 1 |
| process | parameters | dynamicmask | boolean | False | False |
| process | parameters | masknotnullin | integer | False | 255 |
| process | parameters | vectoroverlay | text | False | --- |
| process | parameters | width | integer | False | 0 |
| process | parameters | crop | text | False | --- |
| process | parameters | border | integer | False | 0 |
| process | parameters | bordercolor | text | False | black |
| process | parameters | emboss | text | False | --- |
| process | parameters | embossdims | text | False | 0 |
| process | parameters | embossptsize | integer | False | 0 |
| process | parameters | title | text | False | --- |
| process | parameters | titlesingleline | boolean | False | True |
| process | parameters | titlegravity | text | False | North |
| process | parameters | titlebackgroundcolor | text | False | white |
| process | parameters | titlefontcolor | text | False | black |
| process | parameters | titlefont | text | False | Tahoma |
| process | parameters | titlefontsize | integer | False | 12 |
| process | parameters | detailcrop | text | False | --- |
| process | parameters | detailwidth | integer | False | 0 |
| process | parameters | detailborder | integer | False | 2 |
| process | parameters | detailbordercolor | text | False | black |
| process | parameters | detailtitle | boolean | False | True |
| process | parameters | detaillegend | boolean | False | False |
| process | parameters | detaillegendgravity | text | False | East |
| process | parameters | detaillegendsize | integer | False | 100 |
| process | parameters | detaillegendbackground | text | False | White |
| process | parameters | jpg | integer | False | 0 |
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
| process | srccomp | * | element | True | * |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | True | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcopy | srccomp | text | True | * |
| process | dstcopy | layerid | text | False | copy |
| process | dstcopy | prefix | text | False | copy |
| process | dstcopy | suffix | text | False | copy |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | True | tif |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | overwritelayout | to be completed |
| process | parameters | palette | to be completed |
| process | parameters | minmax | to be completed |
| process | parameters | srcmin | to be completed |
| process | parameters | srcmax | to be completed |
| process | parameters | zscore | to be completed |
| process | parameters | globalmeantozero | to be completed |
| process | parameters | globalmean | to be completed |
| process | parameters | globalstd | to be completed |
| process | parameters | zscorefac | to be completed |
| process | parameters | dynamicmask | to be completed |
| process | parameters | masknotnullin | to be completed |
| process | parameters | vectoroverlay | to be completed |
| process | parameters | width | to be completed |
| process | parameters | crop | to be completed |
| process | parameters | border | to be completed |
| process | parameters | bordercolor | to be completed |
| process | parameters | emboss | to be completed |
| process | parameters | embossdims | to be completed |
| process | parameters | embossptsize | to be completed |
| process | parameters | title | to be completed |
| process | parameters | titlesingleline | to be completed |
| process | parameters | titlegravity | to be completed |
| process | parameters | titlebackgroundcolor | Any color code accpeted by ImageMagick |
| process | parameters | titlefontcolor | to be completed |
| process | parameters | titlefont | to be completed |
| process | parameters | titlefontsize | to be completed |
| process | parameters | detailcrop | to be completed |
| process | parameters | detailwidth | to be completed |
| process | parameters | detailborder | to be completed |
| process | parameters | detailbordercolor | to be completed |
| process | parameters | detailtitle | to be completed |
| process | parameters | detaillegend | to be completed |
| process | parameters | detaillegendgravity | to be completed |
| process | parameters | detaillegendsize | to be completed |
| process | parameters | detaillegendbackground | to be completed |
| process | parameters | jpg | to be completed |
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
| process | srccomp | * | link for source composition |
| process | srcpath | volume | to be completed |
| process | srcpath | hdr | to be completed |
| process | srcpath | dat | to be completed |
| process | dstcopy | srccomp | unknown hint |
| process | dstcopy | layerid | unknown hint |
| process | dstcopy | prefix | unknown hint |
| process | dstcopy | suffix | unknown hint |
| process | dstpath | volume | to be completed |
| process | dstpath | hdr | to be completed |
| process | dstpath | dat | to be completed |

---
layout: subprocess
categories: subprocess
title: ExportTilesToByte
processurl: subprocid-ExportTilesToByte
rootprocid: Export
subprocid: ExportTilesToByte
author: thomasg
excerpt: Export tiles to byte binary
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

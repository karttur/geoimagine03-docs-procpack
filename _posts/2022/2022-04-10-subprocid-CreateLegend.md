---
layout: subprocess
categories: subprocess
title: CreateLegend
processurl: subprocid-CreateLegend
rootprocid: LayoutProc
subprocid: CreateLegend
author: thomasg
excerpt: Create legend for raster layer
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

---
layout: subprocess
categories: subprocess
title: ExportTilesToMap
processurl: subprocid-ExportTilesToMap
rootprocid: Export
subprocid: ExportTilesToMap
author: thomasg
excerpt: Export tiles to map
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
      "processid": "ExportTilesToMap",
      "parameters": {
        "overwriteshade": "False",
        "overwritelayout": "False",
        "palette": "default",
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
        "jpg": "0",
        "palmax": "250",
        "palmin": "0",
        "two51": "False",
        "two52": "False",
        "two53": "False",
        "two54": "False",
        "two55": "False",
        "plotwidth": "8",
        "plotheight": "6",
        "buffer": "10",
        "margin": "10",
        "textpadding": "10",
        "legendposition": "right",
        "legendfitaxis": "True",
        "legendrelativesize": "5",
        "legendpad": "0.5",
        "legendborderpad": "1.5",
        "legendinsetaxis": "False",
        "legendinsetposition": "3",
        "legendrelativewidth": "5",
        "legendrelativeheight": "35",
        "legendheight": "500",
        "legendwidth": "100",
        "soloheight": "70",
        "legendframecolor": "254",
        "legendframefill": "black",
        "legendframestrokewidth": "1",
        "legendticks": "",
        "legendfontcolor": "black",
        "legendfont": "",
        "legendfontsize": "0",
        "legendfonteffect": "",
        "title": "",
        "titleypos": "1.08",
        "titlefontcolor": "black",
        "titlefont": "",
        "titlefontsize": "0",
        "titlefonteffect": "",
        "axisfontcolors": "black,black",
        "axisfont": "",
        "axisfontsize": "0",
        "axisfonteffect": "",
        "majorticks": "0",
        "minorticks": "0",
        "majortickdirection": "inout",
        "majorticklength": "6",
        "majortickwidth": "1",
        "majortickcolors": "black,black",
        "minortickdirection": "in",
        "minorticklength": "2",
        "minortickwidth": "0.5",
        "minortickcolors": "gray,gray",
        "gridcolors": "gray,gray",
        "gridlinestyle": "--",
        "gridlinewidth": "0.5",
        "gridalpha": "0.5",
        "spinecolors": "black,black,black,black",
        "spinelinestyle": "-",
        "spinelinewidth": "0",
        "spinepattern": "",
        "spinexlabels": "",
        "spineylabels": "",
        "northarrow": "",
        "northarrowsize": "0.5",
        "northarrowanchor": "upperleft",
        "northarrowmarginx": "5",
        "northarrowmarginy": "5",
        "northarrowx": "0",
        "northarrowy": "0",
        "logo": "kartturnorth01",
        "logopos": "upperleft",
        "logox": "0",
        "logoy": "0",
        "separatebuffer": "10",
        "columnhead": "",
        "columns": "1",
        "matrix": "False",
        "columntext": "",
        "rowtext": "",
        "rowhead": "",
        "tightlayout": "False"
      },
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
        "hdr": "png",
        "dat": ""
      }
    }
  ]
}
```

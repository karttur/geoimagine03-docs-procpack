---
layout: subprocess
categories: subprocess
title: ExportTilesToMap
processurl: subprocid-ExportTilesToMap
rootprocid: Export
subprocid: ExportTilesToMap
author: thomasg
excerpt: Export tiles to map
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
      "processid": "ExportTilesToMap",
      "parameters": {},
      "srcpath": {
        "volume": ""
      },
      "dstcopy": {
        "srccomp": "*"
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
| process | parameters | overwriteshade | boolean | False | False |
| process | parameters | overwritelayout | boolean | False | False |
| process | parameters | palette | text | False | default |
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
| process | parameters | jpg | integer | False | 0 |
| process | parameters | palmax | integer | False | 250 |
| process | parameters | palmin | integer | False | 0 |
| process | parameters | two51 | boolean | False | False |
| process | parameters | two52 | boolean | False | False |
| process | parameters | two53 | boolean | False | False |
| process | parameters | two54 | boolean | False | False |
| process | parameters | two55 | boolean | False | False |
| process | parameters | plotwidth | float | False | 8 |
| process | parameters | plotheight | float | False | 6 |
| process | parameters | buffer | integer | False | 10 |
| process | parameters | margin | integer | False | 10 |
| process | parameters | textpadding | integer | False | 10 |
| process | parameters | legendposition | text | False | right |
| process | parameters | legendfitaxis | boolean | False | True |
| process | parameters | legendrelativesize | integer | False | 5 |
| process | parameters | legendpad | real | False | 0.5 |
| process | parameters | legendborderpad | real | False | 1.5 |
| process | parameters | legendinsetaxis | boolean | False | False |
| process | parameters | legendinsetposition | integer | False | 3 |
| process | parameters | legendrelativewidth | integer | False | 5 |
| process | parameters | legendrelativeheight | integer | False | 35 |
| process | parameters | legendheight | integer | False | 500 |
| process | parameters | legendwidth | integer | False | 100 |
| process | parameters | soloheight | integer | False | 70 |
| process | parameters | legendframecolor | integer | False | 254 |
| process | parameters | legendframefill | text | False | black |
| process | parameters | legendframestrokewidth | real | False | 1 |
| process | parameters | legendticks | text | False | --- |
| process | parameters | legendfontcolor | text | False | black |
| process | parameters | legendfont | text | False | --- |
| process | parameters | legendfontsize | integer | False | 0 |
| process | parameters | legendfonteffect | text | False | --- |
| process | parameters | title | text | False | --- |
| process | parameters | titleypos | real | False | 1.08 |
| process | parameters | titlefontcolor | text | False | black |
| process | parameters | titlefont | text | False | --- |
| process | parameters | titlefontsize | integer | False | 0 |
| process | parameters | titlefonteffect | text | False | --- |
| process | parameters | axisfontcolors | text | False | black,black |
| process | parameters | axisfont | text | False | --- |
| process | parameters | axisfontsize | integer | False | 0 |
| process | parameters | axisfonteffect | text | False | --- |
| process | parameters | majorticks | integer | False | 0 |
| process | parameters | minorticks | integer | False | 0 |
| process | parameters | majortickdirection | text | False | inout |
| process | parameters | majorticklength | float | False | 6 |
| process | parameters | majortickwidth | float | False | 1 |
| process | parameters | majortickcolors | text | False | black,black |
| process | parameters | minortickdirection | text | False | in |
| process | parameters | minorticklength | float | False | 2 |
| process | parameters | minortickwidth | float | False | 0.5 |
| process | parameters | minortickcolors | text | False | gray,gray |
| process | parameters | gridcolors | text | False | gray,gray |
| process | parameters | gridlinestyle | text | False | -- |
| process | parameters | gridlinewidth | real | False | 0.5 |
| process | parameters | gridalpha | real | False | 0.5 |
| process | parameters | spinecolors | text | False | black,black,black,black |
| process | parameters | spinelinestyle | text | False | - |
| process | parameters | spinelinewidth | real | False | 0 |
| process | parameters | spinepattern | text | False | --- |
| process | parameters | spinexlabels | text | False | --- |
| process | parameters | spineylabels | text | False | --- |
| process | parameters | northarrow | text | False | --- |
| process | parameters | northarrowsize | real | False | 0.5 |
| process | parameters | northarrowanchor | text | False | upperleft |
| process | parameters | northarrowmarginx | integer | False | 5 |
| process | parameters | northarrowmarginy | integer | False | 5 |
| process | parameters | northarrowx | real | False | 0 |
| process | parameters | northarrowy | real | False | 0 |
| process | parameters | logo | text | False | kartturnorth01 |
| process | parameters | logopos | text | False | upperleft |
| process | parameters | logox | real | False | 0 |
| process | parameters | logoy | real | False | 0 |
| process | parameters | separatebuffer | integer | False | 10 |
| process | parameters | columnhead | text | False | --- |
| process | parameters | columns | integer | False | 1 |
| process | parameters | matrix | bool | False | False |
| process | parameters | columntext | text | False | --- |
| process | parameters | rowtext | text | False | --- |
| process | parameters | rowhead | text | False | --- |
| process | parameters | tightlayout | boolean | False | False |
| process | srcpath | volume | text | True | --- |
| process | srcpath | hdr | text | False | tif |
| process | srcpath | dat | text | False | --- |
| process | dstcopy | srccomp | text | True | * |
| process | dstcopy | layerid | text | False | copy |
| process | dstcopy | prefix | text | False | copy |
| process | dstcopy | suffix | text | False | copy |
| process | dstpath | volume | text | True | --- |
| process | dstpath | hdr | text | False | png |
| process | dstpath | dat | text | False | --- |

#### Hints for parameters

| **parent** | **element** | **paramid** | **hint** |
| process | parameters | overwriteshade | to be completed |
| process | parameters | overwritelayout | to be completed |
| process | parameters | palette | to be completed |
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
| process | parameters | jpg | to be completed |
| process | parameters | palmax | to be completed |
| process | parameters | palmin | to be completed |
| process | parameters | two51 | to be completed |
| process | parameters | two52 | to be completed |
| process | parameters | two53 | to be completed |
| process | parameters | two54 | to be completed |
| process | parameters | two55 | to be completed |
| process | parameters | plotwidth | to be completed |
| process | parameters | plotheight | to be completed |
| process | parameters | buffer | to be completed |
| process | parameters | margin | to be completed |
| process | parameters | textpadding | to be completed |
| process | parameters | legendposition | to be completed |
| process | parameters | legendfitaxis | to be completed |
| process | parameters | legendrelativesize | to be completed |
| process | parameters | legendpad | to be completed |
| process | parameters | legendborderpad | to be completed |
| process | parameters | legendinsetaxis | to be completed |
| process | parameters | legendinsetposition | to be completed |
| process | parameters | legendrelativewidth | to be completed |
| process | parameters | legendrelativeheight | to be completed |
| process | parameters | legendheight | to be completed |
| process | parameters | legendwidth | to be completed |
| process | parameters | soloheight | to be completed |
| process | parameters | legendframecolor | to be completed |
| process | parameters | legendframefill | to be completed |
| process | parameters | legendframestrokewidth | to be completed |
| process | parameters | legendticks | to be completed |
| process | parameters | legendfontcolor | to be completed |
| process | parameters | legendfont | to be completed |
| process | parameters | legendfontsize | to be completed |
| process | parameters | legendfonteffect | to be completed |
| process | parameters | title | to be completed |
| process | parameters | titleypos | to be completed |
| process | parameters | titlefontcolor | to be completed |
| process | parameters | titlefont | to be completed |
| process | parameters | titlefontsize | to be completed |
| process | parameters | titlefonteffect | to be completed |
| process | parameters | axisfontcolors | to be completed |
| process | parameters | axisfont | to be completed |
| process | parameters | axisfontsize | to be completed |
| process | parameters | axisfonteffect | to be completed |
| process | parameters | majorticks | to be completed |
| process | parameters | minorticks | to be completed |
| process | parameters | majortickdirection | to be completed |
| process | parameters | majorticklength | to be completed |
| process | parameters | majortickwidth | to be completed |
| process | parameters | majortickcolors | to be completed |
| process | parameters | minortickdirection | to be completed |
| process | parameters | minorticklength | to be completed |
| process | parameters | minortickwidth | to be completed |
| process | parameters | minortickcolors | to be completed |
| process | parameters | gridcolors | to be completed |
| process | parameters | gridlinestyle | to be completed |
| process | parameters | gridlinewidth | to be completed |
| process | parameters | gridalpha | to be completed |
| process | parameters | spinecolors | to be completed |
| process | parameters | spinelinestyle | to be completed |
| process | parameters | spinelinewidth | to be completed |
| process | parameters | spinepattern | to be completed |
| process | parameters | spinexlabels | to be completed |
| process | parameters | spineylabels | to be completed |
| process | parameters | northarrow | to be completed |
| process | parameters | northarrowsize | to be completed |
| process | parameters | northarrowanchor | to be completed |
| process | parameters | northarrowmarginx | to be completed |
| process | parameters | northarrowmarginy | to be completed |
| process | parameters | northarrowx | to be completed |
| process | parameters | northarrowy | to be completed |
| process | parameters | logo | to be completed |
| process | parameters | logopos | to be completed |
| process | parameters | logox | to be completed |
| process | parameters | logoy | to be completed |
| process | parameters | separatebuffer | to be completed |
| process | parameters | columnhead | to be completed |
| process | parameters | columns | to be completed |
| process | parameters | matrix | to be completed |
| process | parameters | columntext | to be completed |
| process | parameters | rowtext | to be completed |
| process | parameters | rowhead | to be completed |
| process | parameters | tightlayout | to be completed |
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

---
layout: post
title: Karttur's GeoImagine Framework Processes
excerpt: "Processes available in Karttur's GeoImagine Framework"
image: rainfall-delta_3B43_trmm_2001-2016_mk-z-ts-model
search_omit: true
---

Karttur's GeoImagine Framework offers a semi-automated processing environment for spatial data, mainly intended for Big Data processing of satellite images and other spatial datasets. To work with the Framework your machine must first be set up with a Spatial Data Integrated Development Environment (SPIDE) as described in my blog on [Install and setup spatial data IDE](https://karttur.github.io/setup-ide/).

At the core of the Framework are object oriented processes. These processes are assembled in groups (called roots), where each group is associated with either a particular data source (e.g. MODIS, Sentinel, Landsat, ancillary etc), or a particular kind of process (e.g. time series processing, scalar, overlay, export etc). Many root processes are also associated with a specific, purpose-built, Python package.

This blog contains all the processes of the Framework.

To search for a particular package or process, use these links to browse the content of Karttur's GeoImagine Framework:

- [Python packages](packages/index.html)
- [Root processes](rootprocesses/index.html)
- [Sub processes](subprocesses/index.html)

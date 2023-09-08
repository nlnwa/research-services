---
title: Maps
layout: home
nav_order: 1
permalink: /docs/maps
---

![](./images/maps-norwebnews.png)

# Map Services
NWA has prototyped a map service that allow geographical exploration of the Norwegian Web Archive. It is currently available for a subset of entities, namely Norwegian Web News (2005-).
{: .fs-6 .fw-300 }

## Norwegian Web News (2005-)
The map for Norwegian Web News represent web news from Spain in the south to Svalbard in the north.

Zoom in/out to find your desired scope. Click on a pin to show the name of the publication. Following the link will make a query for its domain in the archive.

The map is available at the [Norwegian Web Archive's Map of Web News](https://nettarkivet.beta.nb.no/map/)

## Data set
The map service is based on a data set with a register of Norwegian web news sites after 2005., sometimes refered to as 'online newspapers', published between 2005-21.






----

All data about entities and addresses have been extracted from the [Norwegian Entity Register](https://data.brreg.no/enhetsregisteret/api/docs/index.html).

The entities' street addresses have been parsed into geo coordinates, using [Google's Geocoding API](https://developers.google.com/maps/documentation/geocoding/overview).

The map is produced with [QGIS 3.24](https://qgis.org/en/site/), using the [qgis2web](https://github.com/tomchadwin/qgis2web) plugin with [OpenLayers](https://openlayers.org/) and map tiles from [OpenStreetMap](https://www.openstreetmap.org) to produce web resources, with some post-editing of html, css and js.
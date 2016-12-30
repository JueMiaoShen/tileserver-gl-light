# The source code is now part of the original TileServer GL repo: https://github.com/klokantech/tileserver-gl

A light variant of [tileserver-gl](https://github.com/klokantech/tileserver-gl) for serving MBTiles with
[predefined Mapbox GL styles](https://github.com/klokantech/tileserver-gl-styles). Built to support serving vector tiles from [OSM2VectorTiles](http://osm2vectortiles.org/) to modern client.

This trimmed tileserver does not contain server side rendering into raster tiles for legacy clients, GIS and printing, but it is easier to install and without any binary dependencies in npm. It runs everywhere where node.js runs.

For production deploy check the [tileserver-gl](https://github.com/klokantech/tileserver-gl) project and [manual](http://tileserver.readthedocs.io/).

## Get Started

Install `tileserver-gl-light` from npm.

```bash
npm install -g tileserver-gl-light
```

Now download vector tiles from [OSM2VectorTiles](http://osm2vectortiles.org/downloads/).

```bash
curl -o zurich_switzerland.mbtiles https://osm2vectortiles-downloads.os.zhdk.cloud.switch.ch/v2.0/extracts/zurich_switzerland.mbtiles
```

Start `tileserver-gl-light` with the downloaded vector tiles.

```bash
tileserver-gl-light zurich_switzerland.mbtiles
```

## Style and glyphs

The used styles are derived from [Mapbox Open Styles](https://github.com/mapbox/mapbox-gl-styles) and are maintained as npm dependency in a separate repo.

# Version 1.0

We want a Mars globe in the browser. Similar to this [Nasa Mars map](https://trek.nasa.gov/mars/#).

webGL / three.js / [Cesium](https://github.com/CesiumGS/cesium) seem to be the best stack.

Website visitors should be able to

- spin the planet.
- zoom in and out,

When zooming in, load different levels of high res images. For which can use the [Nasa API](https://api.nasa.gov/?search=mars).

# Version 2.0

When we solved the problems above, we want to build new features:

- 3D Tiles: Use elevation data to show the depth of terrain. Like in ([this demo](https://60411c631a034500071134b2--compassionate-hodgkin-5fe53e.netlify.app/)), built in the `threejs` branch (using textures/bump.jpg layer)
- Show geodata like landing sites, from a [a json file like this](mars_landings.geojson).
- Let user choose between different layers / WMTS map source. Like in [this example](https://source.opennews.org/articles/how-we-made-rewind-red-planet), where users can choose between a normal Mars map today, and one with water on the lower surface of Mars.
- Set up our own WMTS map server. Because we don't want to get rate limited by the NASA API, and we want to serve our own images.
- Click one section - like a square of 100 kilometers - to show a black square line around that same area. Similar to this:
![mars_version2](https://user-images.githubusercontent.com/79759818/110023594-a038a800-7d2d-11eb-960c-5660e8b69b12.jpg)

---

## Related links

- Mars globe in react three fiber, using react components. ([Demo](https://6040f862046d3300076eb558--compassionate-hodgkin-5fe53e.netlify.app/)) built from `react` branch.
- Tools for generating map tiles and hosting them: [carto.js](https://github.com/CartoDB/carto.js) or [TileStache](https://github.com/TileStache/TileStache) or [maptiler](https://support.maptiler.com/i70-create-a-3d-online-globe) or upload image files to [Cesium](https://cesium.com/docs/tutorials/uploading/).
- High resolution image tiles, for different layers, from [this page](http://www.celestiamotherlode.net/addon/addon_237.html).
- ([WebGL Earth](http://examples.webglearth.com/#helloworld)), from which I built [this demo](https://60411e2160bdf4000764fe13--compassionate-hodgkin-5fe53e.netlify.app/) on `earth-webgl` branch, using a Mars map from [this API](https://www.openplanetary.org/opm-basemaps/opm-mars-basemap-v0-2).

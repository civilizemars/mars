## Version 1 already working implemented in index.html. See [live demo here](https://thirsty-kirch-dc75b2.netlify.app).

We want a Mars globe in the browser. Similar to this [demo using esri API](https://explore-mars.esri.com/).

Use [these Esri Mars tile maps](https://www.arcgis.com/home/user.html?user=esri_astro) for images and elevation data.

## Feature 2: Grid layer

- Hover area, to
  - show square around area
  - show widget box with information about the area

Three things I want fixed:
- Instead of using [this Grid data](https://github.com/civilizemars/mars/blob/a148bde8f03db2cf7653a5f4caf5b1b2f119f4ea/index.html#L146), I want to use the grid of images I exported from ArcGIS Pro with "Split Raster" tool. See the files in the [`example export`](https://github.com/civilizemars/mars/tree/esri-api/example%20export) folder.
- I don't want to see a popup. So right now I hide the popup with `.esri-popup { visibility: hidden; }`. Maybe it's better to use something like [this example](https://developers.arcgis.com/javascript/latest/sample-code/sandbox/index.html?sample=view-hittest).
- I don't want to see the whole grid of grey squares. I only want to see the one colored square which is hovered. Like ![this](https://i.imgur.com/WEmvzgU.jpg)



## Feature 3: Twitter

- twitter feature (similar as implemented [here](https://explore-mars.esri.com/))
  - send tweet
    - screenshot, coordinates, zoom level and text
  - show tweet on the map
    - coordinates, zoom level, tweet 
![esri twitter](https://i.imgur.com/kASCx9d.png)


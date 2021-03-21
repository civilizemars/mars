## Version 1 already working implemented in index.html. See [live demo here](https://thirsty-kirch-dc75b2.netlify.app).

We want a Mars globe in the browser. Similar to this [demo using esri API](https://explore-mars.esri.com/).

Use [these Esri Mars tile maps](https://www.arcgis.com/home/user.html?user=esri_astro) for images and elevation data.

## Feature 2: Grid layer

- Hover area, to
  - show square around area
  - show widget box with information about the area

Two thing I want fixed:
- I don't want to see the whole grid of grey squares. I only want to see the one colored square which is hovered. Like ![this](https://i.imgur.com/WEmvzgU.jpg)
- I don't want to see a popup. So right now I hide the popup with `.esri-popup { visibility: hidden; }`. Maybe it's better to use something like [this example](https://developers.arcgis.com/javascript/latest/sample-code/sandbox/index.html?sample=view-hittest).


## Feature 3: Twitter

- twitter feature (similar as implemented [here](https://explore-mars.esri.com/))
  - send tweet
    - screenshot, coordinates, zoom level and text
  - show tweet on the map
    - coordinates, zoom level, tweet 
![esri twitter](https://i.imgur.com/kASCx9d.png)

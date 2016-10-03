# MVT Debug

MVT Debug is a single HTML file that is used to test and debug [Mapbox Vector Tiles](https://github.com/mapbox/vector-tile-spec) endpoints. MVT Debug leverages [Open Layers 3](http://openlayers.org/) for rendering.

## Setup
To setup open the index.html file in a code editor and modify the config options at the top of the HTML file. The most important options to set are the view center point and the layer url. Once set, open index.html in a browser and you should see your MVT tiles being rendered.

## Turning on and off layers
MVT Debug will give each feature layer a color and a row in the legend. To turn off a feature layer, click on the feature layer in the legend. The rendering of that layer should switch off in the map. To turn it back on, simply click again.

## Zooming and panning
Zooming and panning around the map will rebuild the legend according to the features that are being rendered in the current viewport. This should help to identify which features are on/off at different zoom levels.

## More layers
Additional layers may be added to the map by adding a new layer to the configuration layers array. MVT Debug will render layers on top of each other using the same coordinates. This may be useful for comparing features on two different endpoints.

## Additional features
On the roadmap for MVT Debug is the ability to control the colors of layers.
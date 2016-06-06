# nyc-trees

NYC street trees rendered dynamically in the landscape architecture hand-drawn tree plan view style.

This was a prototype built during the [NYC TreesCount! Data Jam](https://www.eventbrite.com/e/treescount-data-jam-registration-25235073785) on June 4, 20160.

The data is a subset of the [2015 Tree Census dataset](https://data.cityofnewyork.us/Environment/2015-Street-Tree-Census-Tree-Data/pi5s-9p35), to keep load times and memory footprint smaller. I extracted only the Gramercy Park neighborhood using Chris Whong's [NYC 2015 Street Trees Data Downloader](http://chriswhong.github.io/tree-data-downloader/).

The [data dictionary](https://docs.google.com/spreadsheets/d/1-wbWj5WuQjsQ-uOvfo6NhlUpK8qgIdhS_cXJPvdZ5cQ/edit) is very helpful: I only needed a few columns of data here, and matched the common name of trees with [NYC Parks Approved Species list](https://www.nycgovparks.org/trees/street-tree-planting/species-list) to get a rough idea of tree color. It seems that not all trees are on this list, unfortunately. The matching is _very_ preliminary and the chosen tree art is intended more to show variety than to be visually accurate.

The map is rendered with [Leaflet](http://leafletjs.com/), [Tangram](https://mapzen.com/projects/tangram/), and Mapzen's [Refill map style](https://github.com/tangrams/refill-style/). I dog-fooded [Tangram Play](https://mapzen.com/tangram/play) for working on the scene. The idea is to see if I could use data to render point textures at the appropriate size, and as you can see by playing around the demo, the current method is close, but is still representational in "paper space" than drawn in "model space."

The tree artwork was purchased from [Shutterstock](http://www.shutterstock.com/pic-370545008.html), with a perpetual, worldwide license for unlimited digital reproductions. It is appropriate here, but should not be re-used if this project evolves. I have not included the original JPEG file here only because it is so large.

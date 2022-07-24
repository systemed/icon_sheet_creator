# Icon Sheet Creator

Maplibre GL/Mapbox GL icons are defined by a .png sheet and a JSON index. Creating these sheets from raw icons is fiddly and requires a big stack of Node.

This is a single-file Javascript app onto which you can drop SVG files. You can then click the buttons to generate the JSON index and the .png sheet (at both 1x and 2x resolution).

The SVGs will be rasterised at the width and height you specify in the top bar (specified in pixels for the _2x_ sheet). If you want to specify your own width and (optionally) height, put this in the filename. For example, `cafe|64.svg` would be rasterised at 64px wide. The icon will be named "cafe" in the JSON index.

Richard Fairhurst, 2022. The tilemaker is licensed as FTWPL; you may do anything you like with this code and there is no warranty.
# Icon Sheet Creator

Maplibre GL/Mapbox GL icons are defined by a .png sheet and a JSON index. Creating these sheets from raw icons is fiddly and requires a big stack of Node.

This is a single-file Javascript app onto which you can drop SVG files. You can then click the buttons to generate the JSON index and the .png sheet (at both 1x and 2x resolution).

The SVGs will be rasterised at the width and height you specify in the top bar (specified in pixels for the _2x_ sheet). If you want to specify your own width and (optionally) height, put this in the filename. For example, `cafe|64.svg` would be rasterised at 64px wide. The icon will be named "cafe" in the JSON index.

You can encode `content`, `stretchX` and `stretchY` values like this:

    shield|64|48|x,8,56|y,8,40|c,8,4,54,44.svg

(These coordinates are in the output coordinate space, not the SVG's input space.)

Richard Fairhurst, 2022. This code is licensed as FTWPL; you may do anything you like with this code and there is no warranty.

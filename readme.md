Based off the excellent work from https://github.com/lukasmartinelli/naturalearthtiles

---

This fork from Lukas's work is for

* testing local hosting of raster and vector tiles via `http://localhost:5000` or from a server
 * Open in default browser on localhost
   * `serve . -l 5000`
   * http://localhost:5000/maps/natural_earth.raster.html
   * http://localhost:5000/maps/natural_earth.vector.html
 * If needed, open from roblabs.com (The style favors local over a remote URL, please adjust the style if needed)
   * https://naturalearthtiles.roblabs.com/maps/natural_earth.raster.html
   * https://naturalearthtiles.roblabs.com/maps/natural_earth.vector.html
* Testing of the key `destination` within the key `sources`

```json
"sources": {
    "sr_hr": {
        "destination": "Resources/sr_hr",
        "tiles": [
            "http://localhost:5000/tiles/natural_earth_shaded_relief.raster/{z}/{x}/{y}.png",
            "https://naturalearthtiles.roblabs.com/tiles/natural_earth_shaded_relief.raster/{z}/{x}/{y}.png"
        ],
        "type": "raster",
        "tileSize": 256,
        "maxzoom": 6
    },
    "ne_2_hr_lc_sr": {
        "destination": "Resources/ne_2_hr_lc_sr",
        "tiles": [
            "http://localhost:5000/tiles/natural_earth_2_shaded_relief.raster/{z}/{x}/{y}.png",
            "https://naturalearthtiles.roblabs.com/tiles/natural_earth_2_shaded_relief.raster/{z}/{x}/{y}.png"
        ],
        "type": "raster",
        "tileSize": 256,
        "maxzoom": 6
    },
    "ne_2_hr_lc": {
        "destination": "Resources/ne_2_hr_lc",
        "tiles": [
            "http://localhost:5000/tiles/natural_earth_2.raster/{z}/{x}/{y}.png",
            "https://naturalearthtiles.roblabs.com/tiles/natural_earth_2.raster/{z}/{x}/{y}.png"
        ],
        "type": "raster",
        "tileSize": 256,
        "maxzoom": 6
    },
    "hyp_hr": {
        "destination": "Resources/hyp_hr",
        "tiles": [
            "http://localhost:5000/tiles/natural_earth_cross_blended_hypso.raster/{z}/{x}/{y}.png",
            "https://naturalearthtiles.roblabs.com/tiles/natural_earth_cross_blended_hypso.raster/{z}/{x}/{y}.png"
        ],
        "type": "raster",
        "tileSize": 256,
        "maxzoom": 6
    },
    "hyp_hr_sr": {
        "destination": "Resources/hyp_hr_sr",
        "tiles": [
            "http://localhost:5000/tiles/natural_earth_cross_blended_hypso_shaded_relief.raster/{z}/{x}/{y}.png",
            "https://naturalearthtiles.roblabs.com/tiles/natural_earth_cross_blended_hypso_shaded_relief.raster/{z}/{x}/{y}.png"
        ],
        "type": "raster",
        "tileSize": 256,
        "maxzoom": 6
    },
    "gray_hr_sr": {
        "destination": "Resources/gray_hr_sr",
        "tiles": [
            "http://localhost:5000/tiles/natural_earth_gray_hypso_shaded_relief.raster/{z}/{x}/{y}.png",
            "https://naturalearthtiles.roblabs.com/tiles/natural_earth_gray_hypso_shaded_relief.raster/{z}/{x}/{y}.png"
        ],
        "type": "raster",
        "tileSize": 256,
        "maxzoom": 6
    }
}
```

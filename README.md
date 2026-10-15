# Moon Tracker

A single-file, no-dependencies sky simulator that shows the real position and phase of the moon, the brightest stars and the planets, as seen through a fixed wide-angle "lens" from anywhere on Earth. It starts over Oslo, Norway (59.91°N, 10.75°E).

Made for a 2D game prototype that needs the moon to be in the right place for a real location.

## Features

- Real moon altitude, azimuth, phase and % illuminated
- A little globe: spin it, tap any point (or a city button) and the moon, stars and planets move to that place. It also shows day and night, and where the moon and sun are overhead
- About 105 bright stars, northern and southern sky, and all seven other planets, placed from real coordinates, fading out in daylight
- The ecliptic line, altitude lines and a compass that follows where the lens is aimed
- Turn the lens by dragging, with the slider, or with the buttons
- Time controls: pick a date, jump to now, or play at 1 s/s, 1 h/s, 1 day/s or 1 wk/s
- Works on phones

## Run it

Open `index.html` in a browser. There is nothing to install or build.

To host it free, turn on **GitHub Pages** for the repo (Settings → Pages → deploy from the main branch).

To change the starting location, edit `LAT` and `LON` near the top of the script in `index.html`.

## Accuracy

- Moon: low-precision lunar series, good to a few arc-minutes. It uses the position from Earth's centre, so altitude can be up to about 1° off for an observer on the surface, and it ignores atmospheric refraction.
- Planets: JPL low-precision orbital elements (valid roughly 1800-2050). Saturn's brightness ignores its rings.
- Stars: coordinates were entered by hand and corrected for precession. Spot-check them against a planetarium before relying on them.
- The moon disc is drawn larger than life so it is visible.
- The globe's coastlines are coarse hand-drawn outlines, good for finding a place, not a real map. The point you tap is accurate; the picture around it is not.

This is built for gameplay and visualisation, not navigation.

## Credits

- Lunar series: Jean Meeus, *Astronomical Algorithms*
- Planet elements: E. M. Standish, "Keplerian Elements for Approximate Positions of the Major Planets" (NASA JPL)
- [Shrimpified on GitHub](https://github.com/Shrimpifieddev)

## License

© 2026 Tiny Puddle™. Free to use under the [MIT License](LICENSE).

# 260715_temporal

Demos for the standard date-time API "Temporal". Sample code for the ICS MEDIA article on migrating date handling from `Date` to `Temporal`.

All demos are plain HTML/JS with no build step and use the native `Temporal` directly. No polyfill is loaded, so a browser with native support is required (Chrome / Edge 144+, Firefox 139+). Unsupported environments show a notice at the top of the page.

## Demos

- `docs/01_reservation/` — Salon reservation. Choose an open slot, and see the confirmed booking (`ZonedDateTime`) in the store's time zone and in the visitor's time zone.
- `docs/02_clock-instant/` — World clock. Shows a single instant (`Temporal.Now.instant()`) as the local time of several cities, updating every second.
- `docs/03_dst/` — Time difference. Shows the gap between two cities on a given date, and how Daylight Saving Time changes it between summer and winter.

## Running locally

Serve `docs/` with any static server and open it.

```
npx serve docs
```

## License

MIT License / ICS INC.

## Image credits

Salon photos in `docs/01_reservation/images/` (`tokyo.jpg`, `london.jpg`, `newyork.jpg`) are from [Unsplash](https://unsplash.com/) and used under the [Unsplash License](https://unsplash.com/license) (free for commercial and non-commercial use).

`docs/02_clock-instant/images/worldmap.svg` is a blank world map from [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:World_map_-_low_resolution.svg).

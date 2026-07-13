# 260715_temporal

Demos for the standard date-time API "Temporal". Sample code for the ICS MEDIA article on migrating date handling from `Date` to `Temporal`.

All demos are plain HTML/JS with no build step and use the native `Temporal` directly. No polyfill is loaded, so a browser with native support is required (Chrome / Edge 144+, Firefox 139+). Unsupported environments show a notice at the top of the page.

## Demos

- `docs/01_reservation/` — Salon reservation. Confirms a booking (`ZonedDateTime`) from a store, date, start time, and course, and converts it to the visitor's time zone.
- `docs/02_clock-instant/` — World clock. Shows a single instant (`Temporal.Now.instant()`) as the local time of several cities, updating every second.
- `docs/03_dst/` — Schedule. Shifts an event by hours and shows how `ZonedDateTime` handles a Daylight Saving Time transition.

## Running locally

Serve `docs/` with any static server and open it.

```
npx serve docs
```

## License

MIT License / ICS INC.

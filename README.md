# 260715_temporal

Demos for the standard date-time API "Temporal". Sample code for the ICS MEDIA article on migrating date handling from `Date` to `Temporal`.

All demos are plain HTML/JS with no build step and use the native `Temporal` directly. No polyfill is loaded, so a browser with native support is required (Chrome / Edge 144+, Firefox 139+). Unsupported environments show a notice at the top of the page.

## Demos

- `docs/01_reservation/` — Date-time handling for a reservation system. Builds a confirmed date-time (`ZonedDateTime`) from a reservation date, start time, duration, and store time zone, then converts it to an overseas display time zone.
- `docs/02_clock-instant/` — The contrast between a wall-clock face (`PlainDateTime`) and an exact point in time (`ZonedDateTime`). Shows a single instant across multiple cities at once.
- `docs/03_dst/` — Adding time across a Daylight Saving Time (DST) transition. Shows how the calculation skips a non-existent time and lands correctly.

## Running locally

Serve `docs/` with any static server and open it.

```
npx serve docs
```

## License

MIT License / ICS INC.

# SunSide ☀️

A lightweight web app that calculates which side of a bus or car to sit on to avoid direct sunlight during your journey. Enter your origin, destination, and departure time — it computes the sun's position and your travel bearing to tell you whether to sit left or right.

## How it works

1. Enter your **origin** and **destination** (supports full addresses with street + number)
2. Pick a **date and time** (or hit **Now** to use the current moment)
3. Hit **Calculate** — SunSide will:
   - Geocode both locations via OpenStreetMap Nominatim
   - Compute your travel bearing
   - Calculate the sun's azimuth and elevation using [SunCalc](https://github.com/mourner/suncalc)
   - Tell you whether to sit **left** or **right** to stay in the shade

## Features

- Address autocomplete with street-level precision
- Works anywhere in the world, any time of day
- Handles edge cases: sun below horizon, sun directly ahead/behind
- No backend, no API keys, no install — a single HTML file

## Usage

Open `index.html` directly in any browser. No build step or server required.

## Deploy

Drag the project folder onto [Netlify Drop](https://app.netlify.com/drop) for an instant live URL, or push to GitHub and enable GitHub Pages.

## Tech

- Vanilla HTML, CSS, JavaScript
- [SunCalc](https://github.com/mourner/suncalc) for solar position
- [OpenStreetMap Nominatim](https://nominatim.org/) for geocoding and autocomplete

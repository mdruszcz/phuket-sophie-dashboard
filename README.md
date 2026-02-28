# 🌴 Phuket March — Sophie's Safety Dashboard

Real-time weather forecast & baby-safe activity planner for Phuket, Thailand.

Built for a family trip with a 9-month-old — uses AAP heat index guidelines to classify each hour as **safe**, **caution**, or **danger** for outdoor activities.

## Features

- **3-tier live data**: Google Weather API (AI-powered) → Open-Meteo → embedded snapshot
- **Hourly safety classification** based on apparent temperature / heat index
- **Interactive SVG charts**: temperature, humidity, UV index with tooltips
- **7-day forecast** with day selector tabs
- **Activity recommendations** optimized by time of day
- **Three.js animated background**
- Single self-contained HTML file — no build step

## Safety Criteria (AAP Guidelines)

| Zone | Heat Index | Recommendation |
|------|-----------|----------------|
| 🟢 Safe | < 29°C | Outdoor play OK |
| 🟡 Caution | 29–33°C | Shade & hydrate |
| 🔴 Danger | ≥ 33°C | Stay indoors / AC |

## Usage

Just open `index.html` in a browser. It fetches live forecast data automatically.

To use Google Weather API, add your key in the `GOOGLE_KEY` variable.

## Data Sources

- [Google Weather API](https://mapsplatform.google.com/maps-products/weather/) (primary)
- [Open-Meteo](https://open-meteo.com/) (fallback, CC BY 4.0)
- AAP Heat Index Guidelines (safety thresholds)

## Tech Stack

HTML / CSS / JavaScript / SVG / Three.js — single file, zero dependencies

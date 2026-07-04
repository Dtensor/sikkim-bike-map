# Sikkim & Kalimpong — Biker's Road Atlas 🏍️

**What we built:** a single-file interactive road map of Sikkim + Kalimpong — like a treasure map for motorbikes. Every rideable road is drawn and colour-coded (orange = National Highway, blue = State Highway, green = village road, red-dashed = broken high-altitude track), with distances in km on every segment.

**View it:** https://dtensor.github.io/sikkim-bike-map/

## How I use it
| Action | What It Does | When I Use It |
|---|---|---|
| Open the link above | Loads the full map in any browser | Planning a ride |
| Hover a road | Shows km + condition notes (hairpins, landslides) | Choosing a route |
| Hover a town | Shows altitude, ⛽ fuel, 🛂 permit info | Fuel/permit planning |
| Sidebar checkboxes | Hide/show road classes | "Tarmac only" view |
| Scroll / drag | Zoom and pan | Zooming into the Zuluk hairpins |
| Tap 📍 button | Shows YOUR live blue dot on the map (asks location permission once) | Mid-ride: "where am I vs the next fuel stop?" |

## One real example
Friday night: open the page, untick district roads, see the Old Silk Route loop is ~210 km with last fuel at Rongli, screenshot the permit note, ride out Saturday 7 am.

## What runs automatically
Once you tap 📍, the map keeps updating your blue dot every few seconds by itself — with an accuracy ring, your altitude, the nearest town and how far it is, and a freshness tag ("live" / "2 min ago"). The map auto-follows you as you ride. Tap 📍 again to stop. Needs the HTTPS link (not a downloaded file) — that's a browser safety rule for GPS. 🛰️

*Grown-up note: hand-built single HTML (SVG projected from real lat/lon, Dijkstra-computed hub distances). Distances ±10%; verify permits in Gangtok.*

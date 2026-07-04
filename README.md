# Sikkim & Kalimpong — Biker's Road Atlas 🏍️

**What we built:** a single-file interactive road map of Sikkim + Kalimpong — like a treasure map for motorbikes. Every rideable road is drawn and colour-coded (orange = National Highway, blue = State Highway, green = village road, red-dashed = broken high-altitude track), with distances in km on every segment.

**View it:** https://dtensor.github.io/sikkim-bike-map/
**Frontier map (NEW):** https://dtensor.github.io/sikkim-bike-map/frontier.html — Nepal border to Bhutan border, Kalimpong to beyond Donkya La: 17,826 real OSM ways (16,204 km, incl 2,751 km walking trails), 111 viewpoints, 10 passes, 202 peaks, international borders, 11 permit/army gates, convoy rooms. Toggle **Schematic / Terrain / Satellite** base layers (OpenTopoMap contours + Esri imagery stream in live; schematic works offline).
**Trail map:** https://dtensor.github.io/sikkim-bike-map/kalimpong.html — every small road, jeep track and walking trail within 40 km of Kalimpong (19,907 real OSM ways, ~14,000 km), with 73 ★ viewpoints, a tap-to-measure ruler ⌁ for exact route distances, and the same 📍 live location + 🏍️ ride rooms.

## How I use it
| Action | What It Does | When I Use It |
|---|---|---|
| Open the link above | Loads the full map in any browser | Planning a ride |
| Hover a road | Shows km + condition notes (hairpins, landslides) | Choosing a route |
| Hover a town | Shows altitude, ⛽ fuel, 🛂 permit info | Fuel/permit planning |
| Sidebar checkboxes | Hide/show road classes | "Tarmac only" view |
| Scroll / drag | Zoom and pan | Zooming into the Zuluk hairpins |
| Tap 📍 button | Shows YOUR live blue dot on the map (asks location permission once) | Mid-ride: "where am I vs the next fuel stop?" |
| Tap 🏍️ button | Opens a RIDE ROOM — copy the invite link, friends open it, everyone's dots appear | Group rides: "where is everyone?" |

## One real example
Friday night: open the page, untick district roads, see the Old Silk Route loop is ~210 km with last fuel at Rongli, screenshot the permit note, ride out Saturday 7 am.

## What runs automatically
Once you tap 📍, the map keeps updating your blue dot every few seconds by itself — with an accuracy ring, your altitude, the nearest town and how far it is, and a freshness tag ("live" / "2 min ago"). The map auto-follows you as you ride. Tap 📍 again to stop. Needs the HTTPS link (not a downloaded file) — that's a browser safety rule for GPS. 🛰️

In a ride room 🏍️, your phone quietly shares your position every 12 seconds with your group (only while "broadcasting" is on), and friends' coloured dots update by themselves — even someone joining late instantly sees everyone's last-known spots. No signal in the mountains? The map shows "23 min ago" next to a rider instead of pretending — and resumes on its own when bars come back. 📡

*Grown-up note: hand-built single HTML (SVG projected from real lat/lon, Dijkstra-computed hub distances). Distances ±10%; verify permits in Gangtok.*

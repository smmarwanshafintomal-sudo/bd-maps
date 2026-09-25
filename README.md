# BD Maps 🇧🇩

A Google Maps–style web app **focused only on Bangladesh**.

Interactive map with search, multi-modal directions (Drive / Bus / Walk / Cycle / Fastest), divisions, districts, and popular landmarks — all in English + বাংলা.

![BD Maps](https://img.shields.io/badge/Bangladesh-Only-006a4e?style=flat-square)
![No API Key](https://img.shields.io/badge/No_API_Key-Required-22c55e?style=flat-square)
![OpenStreetMap](https://img.shields.io/badge/Tiles-OpenStreetMap-7c3aed?style=flat-square)

## Features

- **Interactive map** of Bangladesh (OpenStreetMap tiles)
- **Search** — districts, divisions, landmarks (EN + বাংলা), with smart ranking & highlighting
- **Directions** — Fastest / Drive / Bus / Walk / Cycle via OSRM
- **8 Divisions** + **64 Districts** with bilingual names
- **Popular places** — Cox’s Bazar, Sundarbans, Ahsan Manzil, and more
- **My Location** (works when you’re inside Bangladesh)
- Mobile-friendly UI

## How to run

### Option 1 — Open directly
Double-click `index.html` in any modern browser.

### Option 2 — Local server
```bash
python -m http.server 8080
# or
npx serve .
```
Then open http://localhost:8080

## Tech stack

| Part | Source |
|------|--------|
| Map tiles | OpenStreetMap |
| Routing | [OSRM](https://project-osrm.org/) (public demo) |
| Place search | Local data + [Nominatim](https://nominatim.org/) |
| Admin data | Embedded (BD Open API snapshot) |

No API keys required for core features.

## Project structure

```
bd-maps/
├── index.html    # Main page
├── styles.css    # UI styles
├── app.js        # Map, search, routing logic
└── README.md
```

## Notes

- Map view is restricted to Bangladesh bounds
- Bus mode uses the road network (no public GTFS feed available for BD yet)
- Nominatim is used lightly for extra place search when online

## License

MIT — free to use, modify, and share.

Made for Bangladesh 🇧🇩

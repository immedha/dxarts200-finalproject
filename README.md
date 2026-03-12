# Echoes of Visitors

## How to run

No build step or Node.js required. Use either option below.

## Open directly in the browser

Open `map.html` in your browser (double-click the file or drag it into a browser window).

## Project structure

```
echoes-of-visitors/
├── map.html          # Interactive map: click to add pins and location images
├── collage-full.html # Full collage view (mixed sizes, opened via “See full collage”)
├── README.md
└── .gitignore
```

## Technologies and software used

| Technology | Purpose |
|------------|--------|
| **HTML5** | Page structure and semantics |
| **CSS3** | Layout (Grid), styling, responsive behavior |
| **JavaScript** | Map interaction, API calls, DOM updates |
| **Leaflet** (v1.9.4, CDN) | Interactive map: pan, zoom, click handling, markers |
| **OpenStreetMap** | Map tiles (via Leaflet) |
| **Nominatim** (OpenStreetMap) | Reverse geocoding: turn click coordinates into place names (city, state, country) |
| **Wikimedia Commons API** | Search for images by region (state/country) and get thumbnail URLs |
| **localStorage** | Persist collage items so the full collage page can show them |

No frameworks, build tools, or API keys are required. Map and images are loaded from public CDNs and free APIs.

## Features

- **Map:** Click anywhere to add a pin and see the place name and coordinates.
- **Location images:** Each click fetches a photo for the state/country and adds it to the collage strip.
- **See full collage:** Opens `collage-full.html` in a new tab with all images in a mixed-size, slightly rotated layout.
- **Persistence:** Collage data is stored in the browser’s `localStorage` so the full collage reflects your current session.
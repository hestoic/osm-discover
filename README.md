# OpenStreetMap Discover

Find the places you need, right where you are.

OpenStreetMap Discover is a responsive web app that makes it easier to find
nearby places by category, without needing to know a place's exact name.

**Live demo:** https://hestoic.github.io/osm-discover/

## The problem

On the main OpenStreetMap website, finding nearby amenities by category takes
extra effort. Users often have to know a place's name or pan and zoom around
the map. Discover adds a simple, category-first way to explore an area.

## Features

- Category chips for Cafés, Restaurants, Pharmacies, ATMs and Public Toilets
- Search field that filters results as you type
- Interactive map with markers, plus a synchronised results list
- Place details panel with address and opening hours when available
- "Get directions" action for the selected place
- Area search and "use my location" options
- Light and dark themes
- Responsive layout: two-column on desktop, bottom sheet on mobile
- Loading, empty and error states, with form validation and user feedback

## Built with

- HTML5, Tailwind CSS and JavaScript
- [Leaflet](https://leafletjs.com/) for the interactive map
- [OpenStreetMap](https://www.openstreetmap.org/) data and map tiles
- [Overpass API](https://overpass-api.de/) for nearby place data (Fetch API, JSON)
- [Nominatim](https://nominatim.org/) for searching areas by name

## Run it locally

Serve the folder through a local web server rather than opening the file
directly, because OpenStreetMap's tile server blocks pages loaded from `file://`.

    python -m http.server 8000

Then open http://localhost:8000.

## Data notes

Place information comes from OpenStreetMap contributors. Opening hours and
accessibility details are shown only when someone has tagged them, so some
places will have missing details. The app shows a clear message instead of
guessing.

## Credits

Map data © OpenStreetMap contributors, available under the
[Open Database Licence](https://www.openstreetmap.org/copyright).

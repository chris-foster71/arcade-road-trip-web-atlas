# Arcade Road Trip v2026 - static atlas 2026

> **Arcade Road Trip is a web-based static atlas for arcade discovery and route planning, delivering a single-file HTML experience with DuckDB-WASM queries and embedded Parquet data in its current 2026 release.**

[![Platform](https://img.shields.io/badge/Platform-web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/chris-foster71/arcade-road-trip-web-atlas?style=flat-square)](https://github.com/chris-foster71/arcade-road-trip-web-atlas)

---

<p align="center">
  <a href="https://chris-foster71.github.io/arcade-road-trip-web-atlas/">
    <img src="https://img.shields.io/badge/Download-Arcade%20Road%20Trip%20Latest-brightgreen?style=for-the-badge" alt="Download Arcade Road Trip">
  </a>
</p>

> **[Direct Download - Arcade Road Trip v2026](https://chris-foster71.github.io/arcade-road-trip-web-atlas/)**

---

[Download Latest Build](https://chris-foster71.github.io/arcade-road-trip-web-atlas/)

---

## What Arcade Road Trip Is

Arcade Road Trip is a browser-ready atlas centered on arcade venues, trip planning, and hands-on exploration. It is packaged as a static HTML experience, which means the core application can be opened and used directly in the web browser without a conventional install flow.

At its core, the project blends a curated place dataset with a destination overview, a hotspot map, and tools for searching games. That makes it practical for scanning locations, comparing possible stops, and drafting travel routes from embedded data that can be queried in-browser through DuckDB-WASM.

---

## Key Capabilities

- Single-file static HTML app for easy sharing and hosting
- Browser-based DuckDB queries powered by DuckDB-WASM
- Arcade destination dashboard for overview-driven exploration
- Hotspot map for visualizing location clusters and points of interest
- Route planner for building arcade-focused trip paths
- Game search and explore workflow for browsing entries
- Embedded Parquet data for compact, queryable storage
- Static atlas structure that works well in web-first deployments

---

## Getting Started

1. Download or clone the repository.
2. Place the static files on any web server or open the HTML entry point in a browser.
3. If you are serving it locally, start a simple static file server in the project folder.

Example local preview:

    python -m http.server 8000

Then open the app in your browser and load the main HTML page.

---

## How to Use It

Open the atlas in a modern browser and use the dashboard to explore arcade locations, search for games, and inspect mapped hotspots. From there, use the route planner to combine stops into a trip plan that fits your preferred path.

Typical workflow:

1. Load the static HTML app.
2. Search or browse the location database.
3. Review hotspot clusters on the map.
4. Build a route from the destinations you want to visit.
5. Refine your choices using the in-browser query tools.

Because the data is embedded, the app is suited to quick navigation and low-friction exploration from a static deployment.

---

## Configuration Notes

Configuration is typically handled in the static app files or in the embedded data bundle. If you customize the project, look for:

- data source references for the Parquet files
- route or map defaults in the HTML/JS assets
- browser-side query settings used by DuckDB-WASM

Example structure:

    {
      "data": "embedded parquet",
      "mode": "static html",
      "query_engine": "duckdb-wasm"
    }

---

## Requirements

- A modern web browser with JavaScript enabled
- Static hosting support or local file access for the HTML app
- Sufficient browser memory for loading embedded data
- HTML-compatible environment for the single-file interface

---

## FAQ

**How do I refresh the atlas data?**  
Replace or regenerate the embedded Parquet content and update the static HTML bundle.

**Does it need a backend?**  
No. The project is built as a static HTML app and uses browser-side querying.

**Why is DuckDB-WASM included?**  
It allows SQL-style exploration of the location database right in the browser.

**Where are the settings kept?**  
Settings are usually stored in the app assets or in the data/config sections of the static bundle.

**What if the page does not load correctly?**  
Verify that the HTML file and embedded assets are being served properly and that your browser supports the required features.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.

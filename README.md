# GeoServer (deployment)

This folder is a **GeoServer web application + data directory**. GeoServer is an
open-source server for publishing and sharing geospatial data (maps, layers)
over standard OGC web services (WMS/WFS/WCS). The root `index.html` simply
redirects to the admin console at `web/`.

## Contents
- `WEB-INF/`, `META-INF/` — the packaged GeoServer Java web app
- `data/` — the GeoServer data directory (workspaces, layers, styles, config)
- `index.html` — redirect to the admin UI

## Running
Deploy the web app in a servlet container (e.g. Tomcat/Jetty), or run a
standalone GeoServer pointed at this `data/` directory, then open the admin
console (default `http://localhost:8080/geoserver/web/`).

## Notes
- This is a GeoServer instance/data dir, not custom application code.
- See the official GeoServer docs for configuration and service endpoints.

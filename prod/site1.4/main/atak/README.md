# TAK Content Portal (Homelab)

This folder is served read-only via Caddy (internal HTTP) and exposed through NPM (HTTPS) with Authentik SSO.

## Structure
- `packages/`  Mission packages (zip) for offline use
- `overlays/`  KML/KMZ/GPX overlays
- `maps/`      MBTiles / map assets
- `official/`  Official/public datasets (GeoJSON/CAP/etc.)
- `local/`     Personal docs (checklists, comms plan, PDFs)

## Compliance / Safety
- Only store and redistribute datasets that are public and/or explicitly licensed for reuse.
- Avoid rehosting paid/terms-restricted data sources.
- Keep access protected with SSO.

## Publishing workflow (POC)
Drop files into the relevant folder. If this repo is your deployment source of truth, commit and push as normal.
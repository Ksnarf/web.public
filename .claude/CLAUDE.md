# web.public — Claude Context

## What This Repo Is

Static web content and assets for all KSN-hosted domains. This is the **content** side — server config lives in `web.private`.

---

## Directory Map

```
prod/
  site1.0/main/           # ksnarf.com — static HTML
  site1.2/main/           # ksnarf.dev — portfolio + JSON data feeds
    data/
      builds.json         # Featured projects
      inprogress.json     # In-progress experiments
      engagement.json     # Contact info
      site.json           # Site metadata
      status.json         # System status
      now.json            # Current status line
  site1.3/main/           # ksnarf.net
  site1.4/main/           # ksnarf.org + ATAK support
    atak/
      maps/               # Custom map data
      overlays/           # Map overlays
      packages/           # ATAK packages
  site1.5/
    drivein/              # Drive-in event pages
    event/                # Event pages
  [site1.6, site2–5]/
```

---

## Site → Domain Map

| Directory | Domain |
|-----------|--------|
| `site1.0` | ksnarf.com |
| `site1.2` | ksnarf.dev |
| `site1.3` | ksnarf.net |
| `site1.4` | ksnarf.org |
| `site1.5` | ksnarf.download |
| `site1.6` | ksnarf.live |
| `site2` | krissanders.com |
| `site3` | madgwii.com |
| `site4` | outboundtonowhere.com |
| `site5` | exitusrp.com |

---

## ksnarf.dev Data Feeds

`site1.2/main/data/` contains JSON files used as dynamic data sources:
- `builds.json` — Featured project cards (title, description, tech, link)
- `inprogress.json` — Active experiments and WIP
- `now.json` — Short status line shown on the site
- `status.json` — System/service status indicators

When updating project info, edit the JSON files — do not hardcode content in HTML.

---

## Conventions

- All content organized by environment (`prod/`) and site number
- Static files only: HTML, CSS, JS, JSON, SVG, images
- PWA manifest (`manifest.json`) and favicon sets present on main sites
- ATAK support files (maps, overlays, packages) live under `site1.4/atak/`
- Dark theme is the standard visual style across KSN sites

## Adding Content

1. Place files under `prod/site[N]/main/`
2. Match the site number to the domain (see table above)
3. For ksnarf.dev dynamic content, update the relevant JSON in `data/`

## What NOT To Do

- Do not put Caddy server config here — that belongs in `web.private`
- Do not store secrets or `.env` files — this repo is public-facing content
- Do not add server-side code — static files only, served by Caddy

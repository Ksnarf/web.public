# Ktema Wealth Management — ktemawealth.com

Static marketing site for Ktema Wealth Management, the Finance/Fiduciary
brand under Foundry. Single self-contained `index.html` — no build system,
no framework, no runtime data fetching. Open it directly or serve the
`prod/site6/main/` directory statically.

## Files
- `index.html` — the entire site (inline CSS + minimal vanilla JS).
- `assets/noise.svg` — subtle background texture.
- `ver` — version string.
- `LICENSE.md`

## Account login
The "Account Login" / "Client Login" buttons open a vanilla-JS modal
styled as an institutional client portal. It is **non-functional** —
form submit is prevented and portal integration is pending (see TODOs).

## TODO (placeholders to fill before launch)
- AUM figure (`$X.XB`) — use a real, compliance-approved number or remove.
- Phone, mailing address.
- Compliance disclosures / RIA registration details + CRD #.
- Insights articles (3 placeholders).
- Client-portal URL + auth backend wiring.
- Contact form backend (currently `action="#"`).
- Consultation booking link.
- Compliance-counsel review of ALL disclosure / fiduciary language.

## Disclaimer
Nothing in this repo is investment advice. Regulatory/disclosure text is
placeholder and must be reviewed by compliance counsel before publishing.

# Wealth-Management Web Design — Best-Practices Benchmark

**Date:** 2026-06-27
**Method:** Scraped 15 top wealth-management / advisory homepages (design + copy) and distilled the recurring patterns. Source firms below. Used to guide the Ktema Wealth Management site (`prod/site6`).

## Firms benchmarked
Fisher Investments · Creative Planning · Mariner Wealth Advisors · Edelman Financial Engines · Mercer Advisors · Wealthfront · Betterment · Empower · Facet · Savant Wealth · Carson Group · Wealth Enhancement Group · Vanguard Personal Advisor · Brown Advisory · Buckingham/Focus Partners.

> Segment split: traditional RIAs (Fisher, Creative Planning, Mariner, Mercer, Savant, WEG, Brown) vs. roboadvisor/fintech (Wealthfront, Betterment, Empower, Facet). Ktema should follow the **traditional-RIA** playbook, borrowing a little fintech polish.

---

## 1. Visual system

| Pattern | What the leaders do | Verdict for Ktema |
|---|---|---|
| **Palette** | One confident brand color + neutrals. RIAs skew cool/heritage (Creative Planning teal `#165D7D`, Brown navy, Vanguard red-on-white) or warm-earthy (Mariner sand+blue+burnt-orange, WEG olive `#445937`+rust+gold). Fintechs go bolder (Mercer magenta `#c00686`, Wealthfront blurple, Betterment navy+gold `#ffc729`). | Navy + single gold accent is squarely on-pattern (mirrors Betterment navy/gold, Brown navy). Keep it. |
| **Typography** | **Serif heading + sans body** is the dominant RIA signal — 4 of 5 traditional firms (Mencken/AttenNew, Source Serif 4/Inter, Merriweather/IBM Plex Sans, Source Serif Pro/Nimbus Sans). Fisher (all-sans) is the outlier. | Ktema already does serif-head/sans-body — correct. Consider a real serif (Source Serif / Merriweather) over Georgia for premium feel. |
| **Whitespace & density** | Generous whitespace, calm density, large hero type (Betterment 72px H1). | Ktema matches. |
| **Imagery** | Warm life-stage human photography (couples, retirees, families) is near-universal for RIAs. Fintechs use UI screenshots + charts instead. Brown/Vanguard lean minimal. | **Gap:** Ktema has zero photography. Add 1–2 tasteful human/lifestyle or abstract images (hero side or about). Biggest single visual lift. |
| **Motion** | Subtle — card hovers, light parallax, occasional video hero (Focus Partners). Never flashy for RIAs. | Ktema's hover lifts are enough. Don't add more. |

## 2. Layout & section order (the canonical RIA homepage)

Near-universal order across the 15:

1. **Sticky top nav** — wordmark left; anchor links + **Client Login** (top-right utility) + one soft CTA.
2. **Hero** — one confident headline + short subhead + 1–2 CTAs. Often a stat row baked into the hero (Edelman).
3. **Trust strip** — AUM + awards + advisor/client counts, *immediately* below hero. **This is the most consistent pattern of all 15.**
4. **Segmentation or value pillars** — net-worth tiers (Creative Planning: Ultra-Affluent / HNW / Retirement) or 4 "your team/portfolio/firm" pillars (Mercer).
5. **About / philosophy** — fiduciary conviction, firm story.
6. **Services grid** — 6–8 cards w/ line icons (universal).
7. **Process** — 3–4 numbered steps (Discover/Design/Implement/Steward; Listen/Craft/Guide; Start/Match/Plan).
8. **Insights / Views & News** — 3 article cards.
9. **CTA band** — single soft consultative line + button.
10. **Contact / advisor-locator + lead form**, then **mega-footer** with heavy compliance.

Ktema already follows ~8 of these 10. **Missing: (4) audience segmentation, and a near-hero trust placement variant.**

## 3. Language & messaging

- **Tone:** confident + warm. RIAs pair gravitas ("disciplined," "fiduciary," "built to last") with human warmth ("for you," "the life you're building," "people people"). Avoid jargon.
- **Headline formula:** short, benefit-led, often second-person. Examples: "Where your wealth goes *next* is up to you." (Mariner) · "Your future is our focus™." (Focus) · "The confidence that comes with a dedicated advisor" (Vanguard).
- **Fiduciary word:** RIAs say it outright (Savant: "fee-only, fiduciary firm"; Creative Planning: "Fiduciary Wealth Management"). Fintechs avoid it and say "SEC-registered investment adviser" instead. **Ktema is an RIA → say "fiduciary" prominently. Already does.**
- **Trust signals (the formula, near-universal):** `AUM figure + Barron's/WSJ/Newsweek/USA Today award(s) + advisor/client counts + fiduciary claim` — high on the page. Every single RIA does this.
- **Proprietary process names** add premium feel (WEG "Plan-led investing™ / the Roundtable™"; Savant "Wise Counsel / Ideal Futures®"). Optional for Ktema.
- **CTA verbs:** one soft primary CTA repeated — "Schedule a Consultation" / "Let's Talk" / "Get started" / "Let's Chat." Ktema's "Schedule a Consultation" is on-pattern.

## 4. Account / client login (specifically requested)

- **Placement:** top-right utility bar — unanimous across all 15.
- **Label split:** traditional RIAs use **"Client Login"** (Fisher, Mariner, Savant) or **"CLIENT LOGIN"** uppercase (Brown), or **"Client Logins"** plural when multiple custodians (Edelman, Savant, Focus — they link Schwab/Fidelity portals separately). Fintechs use lowercase "Log in."
- **Pattern:** login is almost always a **link out to a separate portal** (`portal.firm.com`, custodian SSO), not an inline modal. Several list **multiple** logins (firm portal + Schwab + Fidelity + 401k).
- **Implication for Ktema:** "Account Login" is fine, but **"Client Login"** is the more institutional RIA label. The modal is good for a static demo; production should point to a real portal URL (and optionally list custodian logins).

## 5. Compliance (table-stakes, every site)

Every firm's footer carries: RIA registration statement, Form ADV Part 2A + Form CRS links, award methodology/"no compensation paid" disclaimers, CFP®/CFA® trademark notices, "not investment advice / past performance" language. Savant even warns against off-channel (WhatsApp/Telegram) impersonation. **Ktema's footer has the skeleton but needs the ADV/CRS links + award disclaimers once real.**

---

## Scorecard — Ktema vs. benchmark

| Dimension | Status |
|---|---|
| Navy + single accent palette | ✅ on-pattern |
| Serif head / sans body | ✅ (upgrade font optional) |
| Sticky nav + top-right login | ✅ |
| Hero + dual CTA | ✅ |
| Trust strip w/ AUM+fiduciary | ✅ structure (needs real numbers/awards) |
| Services grid + icons | ✅ |
| Numbered process | ✅ |
| Insights cards | ✅ (placeholder) |
| CTA band + contact + footer compliance | ✅ skeleton |
| **Human/lifestyle imagery** | ❌ missing |
| **Audience segmentation block** | ❌ missing |
| **Awards/recognition row** | ❌ missing |
| **"Client Login" label + portal/custodian pattern** | ⚠️ uses "Account Login", modal-only |
| **Real serif font** | ⚠️ Georgia stand-in |
| **ADV/CRS links + award disclaimers** | ⚠️ placeholder only |

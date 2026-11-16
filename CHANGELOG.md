# Changelog — silentfam.com

Every change below is a git commit in this repository; this file is the readable version of that history.
Dates are KST. Newest first.

## 2026-11-16

**Design system**
- Floating pill header, matching SilentQuants: capsule navigation over the page, language switch, theme toggle
  and a link across to SilentQuants.
- Wordmark split into two halves: `Fam` carries the accent; on hover the halves swap colour, tighten and
  scale to 1.07. Same treatment for keyboard focus.
- Light theme stays opt-in; dark remains the default for anyone with no stored preference.

**Language**
- Korean rewritten to sound spoken rather than translated: `유명해지고 싶은 게 아닙니다. 자유롭고 싶은 겁니다.`
- Navigation: 왜 · 무엇을 · 어떻게 · Contact.
- Section labels: 01 왜 / 02 무엇을 만들고 있나 / 03 어떻게 하고 있나 / 04 여정 / 05 서한 / 06 Contact.

**Sections**
- Journey rewritten as six chapters, written out at length (one rule before any tool · two systems · the
  family-data boundary · hardening week · the database admitting gaps · this build). A personal family entry
  was tried and removed: the family story belongs to SilentQuants.
- Numbers in the stats row count up when they enter the viewport, with a safety timer so they always land on
  the true value, and no animation for `prefers-reduced-motion`.

**Content honesty**
- Helix named as `Helix — prop firm & broker database`.
- Letters section announces what is being written instead of inventing two published letters.
- Privacy page rebuilt in the same design; footer claim corrected from "no analytics" to "no tracking" to
  match the policy (Cloudflare Web Analytics is cookieless and aggregate).

**Infrastructure**
- Site served from this repository via GitHub Pages on `silentfam.com` (EN at `/`, Korean at `/ko/`), with
  Cloudflare in front for TLS; www redirects to the apex.

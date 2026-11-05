# Vella Cars — vellacars.com (static landing site)

The automotive UGC desk of **influUGC**. Built Nov 6, 2026. **Files only — not deployed.**

## ⚠️ Content model + design direction (owner orders, Nov 5–6, 2026)

- **Content-first (owner update, Nov 6, 00:24):** network sites must NOT be pure
  company brochures. They lead with useful **content** — tips, guides and
  information that search engines and AI answers surface and that brings
  traffic — with influUGC's services and real work woven inside the content,
  and the central CTAs doing the conversion. This site applies the model: the
  homepage carries a full **"Guides for automotive marketers"** section
  (3 substantive starter guides, below) ahead of the services list, and each
  guide closes with a soft woven-in influUGC line + the standard central CTA.
- **Identity (owner order, Nov 5, 23:57):** ALL network satellite sites use the
  main influUGC identity — black background `#000`, neon lime accent `#C8FF00`,
  dark panels, bold heavy typography, the www.influugc.com feel.
- Brand lockup: `Vella Cars.` wordmark with the subline "UGC & content for
  automotive by influUGC" (Arabic: «UGC ومحتوى للسيارات من influUGC»).
- Only real company data: est. 2020, Arab League St Agouza (Giza 12651),
  Egypt + Saudi/Gulf, real client names (Riyadh Season, Saudi Tourism
  Authority, flynas, Saudia, realme, Domino's, TikTok Live, Zanussi).
  No prices, no invented figures, specifications or statistics, no
  testimonials, no stock imagery (CSS/text only).

## Pages built (3 HTML pages, 2 languages)

| File | What |
|---|---|
| `index.html` | English-first landing (LTR): hero, client proof strip, **Guides for automotive marketers** (3 starter guides, anchor-linked), 5 services (dealer & showroom UGC, review-style creator content, launch & test-drive event content, after-sales & service-centre content, monthly packs), 4-step how-it-works, deliverables checklist, why influUGC (with the in-body editorial link to influugc.com), 6-question answer-first FAQ, contact/CTA band, network footer. |
| `ar.html` | Full Arabic mirror (RTL), same structure, guides and FAQ. |
| `404.html` | Branded not-found page (English). |

Plus: `styles.css`, `favicon.svg` (black + lime VC mark), `sitemap.xml`
(hreflang-annotated), `robots.txt`, `llms.txt`, `render.yaml`.

### The 3 starter guides (on-page sections, both languages)

1. `#guide-brief` — **How to brief a creator for a car review video**: access
   and responsibility settled in writing first (exact car/trim, filming
   window, authorised licensed drivers only, insurance & safety in general
   terms under the dealer/brand's own rules, safety before any shot,
   condition/care and return); the **approved claims list** — documented
   facts only, official figures from the car's own documentation,
   impressions free but performance/consumption/safety claims only from
   the list; why keys + a verbal "make something nice" fails.
2. `#guide-testdrive` — **Test-drive content that answers buyer questions**:
   space shown not quoted, consumption handled honestly (varies with
   conditions; official documented figures only — never invent a number),
   tech used not described, ownership questions from published terms, end
   with the next step. Explicit in-guide rule: no number that is not in the
   car's official documentation goes in the video. No specs anywhere.
3. `#guide-launch` — **UGC for car launches in Egypt & Saudi Arabia**: what
   to film (the reveal, first reactions, the questions corner, the event
   context) and **embargo discipline** — written brief before the event,
   nothing published before the agreed reveal moment, access per
   accreditation, approval flow; social-first, vertical-first, Arabic-first
   creators; the market calendar in the date conversation.

Each guide ends with a soft woven-in line (influUGC runs exactly this for
automotive clients) + the standard book/WhatsApp CTAs with
`utm_source=vellacars`.

## SEO / GEO

- Canonical base `https://vellacars.com/` (the real domain; if this site is
  first deployed to an `onrender.com` URL before the domain attaches, switch
  all canonical/OG/sitemap/robots/llms bases in one pass, same as the
  ugccompany rule in `../DEPLOY.md` §2).
- Title/meta target "UGC & content marketing for automotive" + Egypt /
  Saudi Arabia in both languages; OpenGraph + Twitter cards; hreflang
  ar/en both ways.
- JSON-LD: `Organization` (with `parentOrganization: influUGC`, postal
  address, areaServed, the four real social profiles), `WebSite`, and
  `FAQPage` matching each page's visible FAQ.

## CTAs (both carry the satellite UTM set)

- Booking → `https://www.influugc.com/book?utm_source=vellacars&utm_medium=satellite&utm_campaign=network`
- WhatsApp (client line) → `https://wa.me/201029979797?utm_source=vellacars&utm_medium=satellite&utm_campaign=network`
- Footer legal line: "Part of the influUGC network" linking to the hub.

## What remains (not done here)

1. **Deploy** — static folder; Render Static Site (free tier per the network
   rule). The repo's `render.yaml` blueprint pre-fills the service name
   (`vellacars`) and publish path (`.`). Expected live URL once created:
   https://vellacars.onrender.com
2. **Domain attach** — point `vellacars.com` DNS at the host (same checklist
   pattern as `../DEPLOY.md` §4: apex A + www CNAME from the host's screen;
   no MX changes — mail stays on influugc.com).
3. **Marketplace note:** vellacars.com was pulled from the $200 sale tier
   into the network by the owner's Nov 6 activation order — if a $200
   listing still exists anywhere for it, it must come off before traffic is
   pointed at the domain.
4. After go-live: dedicated Google Search Console property + submit
   `sitemap.xml`; verify both pages return 200, the guides render, and the
   FAQ matches the JSON-LD.

## Deploy status (Nov 6, 2026)

- **Repo**: https://github.com/mostafaabaas/vellacars (PUBLIC from birth, per
  the Nov 6 activation design; branch `main`) — source pushed Nov 6, 2026.
- **Hosting**: PENDING-DASHBOARD — the Render Static Site service has **not**
  been created yet; creation happens in the parent activation wave.

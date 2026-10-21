# SEO Strategy: Rymarstwo Marcin Nowak, Tapicer Samochodowy

Mode: rebuild of an existing site (static 2017 site by Coldlight Creative). No live crawl, rank or traffic data was pulled; there are no API credentials, so baselines are set in week 1 (see KPIs).

## Business snapshot

- **What:** car upholstery specialist with leather, classic-car interiors, steering wheels, headliners, convertible roofs, motorcycle seats, antique furniture and horse-drawn vehicles.
- **Where:** a workshop in Krzyszkowice (powiat myślenicki). Serves Kraków and Myślenice.
- **Edge:** family saddlery tradition since 1998, own firm since 2004, a Cadillac limousine restoration using fabrics from an original pattern book. No competitor in the research has this story.
- **Weak spots:** contact info is thin (no hours online until now, no email, no social link), the 2017 footer makes the site look abandoned, Google Maps data is unverified, and 4.1★/22 on Nicelocal includes complaints about long waits.

## Goals

1. Rank in the local pack and top 5 organic for "tapicer samochodowy Kraków" and "tapicer samochodowy Myślenice".
2. Own the niche queries: classic-car upholstery ("tapicerka samochodów zabytkowych", "renowacja wnętrza klasyka") across Małopolska and ideally nationwide, because classic owners travel.
3. More phone calls from organic and GBP. Calls are the KPI, not traffic.
4. Fix the trust gap: fresh site, consistent NAP, real reviews, honest expectations about booking ahead.

## Target audiences

| Segment | Need | Lands on |
|---|---|---|
| Daily-car owner, Kraków / Myślenice | worn steering wheel, sagging headliner, torn seat | service page, location page |
| Classic / youngtimer owner (whole Poland) | faithful interior restoration | `/uslugi/renowacja-samochodow-zabytkowych/`, `/realizacje/` |
| Motorcyclist | seat re-cover | `/uslugi/motocykle/` |
| Antique furniture / carriage owner | rare craft | `/uslugi/renowacja-mebli-antycznych/`, `/uslugi/pojazdy-konne/` |

## Keyword pillars

Volumes not measured. Run them through Google Keyword Planner or DataForSEO before finalising priorities.

1. **Local core:** tapicer samochodowy Kraków / Myślenice, tapicerstwo samochodowe Kraków, tapicer samochodowy Małopolska
2. **Steering wheels:** obszycie kierownicy skórą (Kraków), kierownica alcantara, obszycie kierownicy cena
3. **Classic cars:** tapicerka samochodów zabytkowych, renowacja tapicerki klasyka, tapicer oldtimer
4. **Components:** wymiana podsufitki, dach kabrio, obszycie deski rozdzielczej, gałka zmiany biegów skóra, mieszek
5. **Heritage niche:** rymarstwo, tapicer bryczki, renowacja mebli antycznych Kraków

## On-page rules

- Title format: `<Usługa> – Tapicer samochodowy Kraków, Myślenice | Marcin Nowak`, under 60 characters where possible.
- One H1 per page that matches the primary keyword. The meta description ends with the phone number.
- Original photos only, with descriptive Polish alt text, WebP/AVIF, and explicit width/height.
- Every service page has: what's done, materials (leather types, perforation, alcantara), 3 projects, "Jak wygląda zlecenie" (process + booking ahead), FAQ block, call CTA.

## E-E-A-T plan

- **Experience:** before/after photo sets on every project page. Ask the client for photos (`assets/`).
- **Expertise:** About page in Marcin's own voice with the 1998 → 2004 timeline and the carriage-to-car story. Name materials and techniques concretely.
- **Authority:** classic-car clubs, rally and zlot listings, mentions from restoration forums (see roadmap Phase 3–4).
- **Trust:** full NAP, NIP/REGON once confirmed, privacy policy, a review page linking to sources, honest lead-time wording, and a current-year footer.

## Technical foundation

- Static site generator (Astro / Eleventy) or plain HTML. No CMS is needed for about 25 pages. Host on a CDN with HTTPS and one canonical host.
- Core Web Vitals targets: LCP < 2.5 s, INP < 200 ms, CLS < 0.1 on mobile 4G.
- `robots.txt` allows all, including AI crawlers (GPTBot, ClaudeBot, PerplexityBot), and references the sitemap.
- JSON-LD per page type, as in `SITE-STRUCTURE.md`. Base entity:

```json
{
  "@context": "https://schema.org",
  "@type": "AutoRepair",
  "@id": "https://tapicer-samochodowy.pl/#business",
  "name": "Rymarstwo – Marcin Nowak, Tapicer samochodowy",
  "url": "https://tapicer-samochodowy.pl/",
  "telephone": "+48605304999",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "Krzyszkowice 320A",
    "addressLocality": "Krzyszkowice",
    "postalCode": "32-445",
    "addressRegion": "małopolskie",
    "addressCountry": "PL"
  },
  "openingHoursSpecification": [{
    "@type": "OpeningHoursSpecification",
    "dayOfWeek": ["Monday","Tuesday","Wednesday","Thursday","Friday"],
    "opens": "08:00", "closes": "17:00"
  }],
  "areaServed": ["Kraków", "Myślenice"],
  "founder": { "@type": "Person", "name": "Marcin Nowak" },
  "foundingDate": "2004"
}
```

Add `geo` from the GBP pin. Leave out `priceRange`, `email` and `sameAs` until confirmed.

## Local SEO

- **Google Business Profile:** claim and verify it (video verification). Primary category "Tapicer samochodowy" (Car upholsterer), secondary "Rymarz" if available. Add the hours above, 30+ original photos, and a services list matching the `/uslugi/` pages. Post monthly with a project photo.
- **Citations:** make NAP identical on Cylex, pkt.pl, Panorama Firm, biznesfinder, Oferteo, dobrymechanik.pl, Apple Maps and Bing Places. Fix the "320a"/"320A" and phone-format variations.
- **Reviews:** after each finished job, send a short-link to Google reviews. Reply to every review, negative ones too, politely and without arguing. Never buy or write reviews.

## AI search (GEO)

- Quotable answers: each FAQ answer is 40–80 words and self-contained, e.g. "Ile trwa obszycie kierownicy?" answered honestly.
- A clear entity: the same name, founder, address and dates on site, GBP and directories.
- Get onto "best tapicer in Kraków" lists (Oferteo, local blogs). This is the top AI-visibility factor per the template.

## KPIs

Baselines are measured in week 1 from GSC, GBP Insights and a manual rank check.

| Metric | Baseline | 3 mo | 6 mo | 12 mo |
|---|---|---|---|---|
| Organic clicks / mo (GSC) | measure | +30% | +75% | 2× |
| GBP calls / mo | measure | +25% | +50% | 2× |
| "tapicer samochodowy Kraków" position | measure | top 10 | top 5 | top 3 / local pack |
| Classic-car pillar keywords in top 10 | measure | 2 | 5 | 10 |
| Google reviews | measure | +5 | +12 | +25 |
| Indexed pages | ~old site | 25 | 35 | 50 |
| CWV (mobile, all good) | measure | pass | pass | pass |

## Risks

| Risk | Mitigation |
|---|---|
| Losing rankings from old .html URLs | Full redirect map from a pre-launch crawl; watch GSC 404s for 4 weeks |
| Review complaints about waits | Honest "terminy ustalamy z wyprzedzeniem" copy, reply to reviews, no speed claims |
| Thin per-make or location pages | Quality gates in `SITE-STRUCTURE.md`; merge rather than publish thin |
| Client can't supply photos or copy | Phase 1 uses existing site photos (with permission); photo day in Phase 2 |
| Unconfirmed facts leak into copy | All [CONFIRM] items blocked until answered |

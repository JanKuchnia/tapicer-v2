# Site Structure: tapicer-samochodowy.pl

Template: `local-service` (claude-seo). Built from `brief.md` and `research.md`; anything marked [CONFIRM] there stays unconfirmed here.

## Principles

- **Polish only.** All slugs and copy in Polish. Slugs are lowercase ASCII with no diacritics (`ł` → `l`, `ś` → `s`), and no `.html`.
- **Keep old URLs alive.** The 2017 site has per-make and per-service pages that are already indexed. Every old URL gets a 301 to its new equivalent (map below). Nothing is dropped without a redirect.
- **Phone is the conversion.** Every page has a tap-to-call `605 304 999` and the hours (Mon–Fri 08:00–17:00) above the fold on mobile.
- **No prices, no speed claims.** Quotes stay "zadzwoń po wycenę". Never write "szybko" or "zawsze na czas" (see review sentiment). Say honestly that booking ahead is needed.
- **Heritage is the differentiator.** Family saddlery since 1998, horse-drawn carriages, then cars. Competitors don't have this, so it belongs on the homepage, About, and classic-car pages.

## URL hierarchy

```
/                                         Strona główna
├── /uslugi/                              Usługi (hub)
│   ├── /uslugi/tapicerka-samochodowa/    Seats & full interiors, passenger cars
│   ├── /uslugi/renowacja-samochodow-zabytkowych/   Classic car interiors (flagship)
│   ├── /uslugi/obszywanie-kierownic/     Steering wheels: leather, perforated, alcantara, airbag cover
│   ├── /uslugi/podsufitki/               Headliners + side pillars
│   ├── /uslugi/dachy-kabrio/             Convertible roofs
│   ├── /uslugi/deski-rozdzielcze/        Dashboards
│   ├── /uslugi/drobne-elementy/          Gear knob, gaiters, handbrake, armrest, door seals
│   ├── /uslugi/motocykle/                Motorcycle seats & helmets
│   ├── /uslugi/renowacja-mebli-antycznych/   Antique furniture
│   └── /uslugi/pojazdy-konne/            Horse-drawn vehicles & saddlery (rymarstwo)
├── /realizacje/                          Portfolio (hub, filter by make/service)
│   ├── /realizacje/cadillac-limuzyna/    Featured: full Cadillac limousine restoration
│   ├── /realizacje/<marka>-<model>/      One page per real project (see quality gate)
│   └── ...
├── /obszar-dzialania/                    Service area (hub)
│   ├── /obszar-dzialania/krakow/
│   └── /obszar-dzialania/myslenice/
├── /o-firmie/                            About: Marcin Nowak, 1998 → 2004 → today
├── /opinie/                              Reviews (real ones only, linked to source)
├── /cennik/                              How pricing works (no numbers): what drives cost, how to get a quote
├── /faq/                                 Pytania i odpowiedzi
├── /poradnik/                            Blog (launch in Phase 2)
│   └── /poradnik/<slug>/
├── /kontakt/                             NAP, map, hours, phone, form
└── /polityka-prywatnosci/                Required for the contact form (RODO)
```

Total at launch: about 25 indexable pages. Blog and extra portfolio pages are added later.

## Page specs

| Page | Primary keyword (PL) | Intent | Min words | Schema |
|---|---|---|---|---|
| `/` | tapicer samochodowy Kraków | local / commercial | 600 | `AutoRepair` (LocalBusiness subtype), `Organization`, `WebSite` |
| `/uslugi/` | tapicerstwo samochodowe usługi | navigational | 300 | `ItemList`, `BreadcrumbList` |
| `/uslugi/tapicerka-samochodowa/` | tapicerka samochodowa, obszycie foteli skórą | commercial | 800 | `Service` + `provider` → business |
| `/uslugi/renowacja-samochodow-zabytkowych/` | tapicerka samochodów zabytkowych, renowacja wnętrza klasyka | commercial | 1000 | `Service` |
| `/uslugi/obszywanie-kierownic/` | obszycie kierownicy skórą Kraków | commercial | 800 | `Service`, `FAQPage` content block |
| `/uslugi/podsufitki/` | wymiana podsufitki | commercial | 600 | `Service` |
| `/uslugi/dachy-kabrio/` | dach kabrio wymiana / naprawa | commercial | 600 | `Service` |
| `/uslugi/deski-rozdzielcze/` | obszycie deski rozdzielczej | commercial | 600 | `Service` |
| `/uslugi/drobne-elementy/` | obszycie gałki zmiany biegów, mieszek | commercial | 600 | `Service` |
| `/uslugi/motocykle/` | tapicer motocyklowy, obszycie siedzenia motocykla | commercial | 600 | `Service` |
| `/uslugi/renowacja-mebli-antycznych/` | renowacja mebli antycznych tapicer | commercial | 600 | `Service` |
| `/uslugi/pojazdy-konne/` | rymarstwo, tapicerka bryczki | commercial / niche | 600 | `Service` |
| `/realizacje/` | realizacje tapicer samochodowy | browse | 300 + grid | `CollectionPage`, `ItemList` |
| `/realizacje/<project>/` | `<marka> <model> tapicerka` | proof | 300 + 6+ photos | `CreativeWork`, `ImageObject` |
| `/obszar-dzialania/krakow/` | tapicer samochodowy Kraków | local | 600, 60% unique | `AutoRepair` with `areaServed` |
| `/obszar-dzialania/myslenice/` | tapicer samochodowy Myślenice | local | 600, 60% unique | `AutoRepair` with `areaServed` |
| `/o-firmie/` | Marcin Nowak tapicer rymarz | trust | 600 | `AboutPage`, `Person` (founder) |
| `/opinie/` | opinie tapicer Krzyszkowice | trust | — | `Review` items only if hosted first-party (no self-serving `AggregateRating`) |
| `/cennik/` | ile kosztuje obszycie kierownicy / tapicerka cena | informational | 500 | `FAQPage`-style Q&A (no rich result expected) |
| `/faq/` | — | informational | 600 | none needed (FAQ rich results are restricted); clean Q&A HTML for AI citation |
| `/kontakt/` | tapicer Krzyszkowice kontakt | navigational | 200 | `ContactPage`, `AutoRepair` |

## Service area: kept deliberately small

Only **Kraków** and **Myślenice** are confirmed (they are in the old site title). More towns (Wieliczka, Dobczyce, Niepołomice; competitor Skórzana Alchemia targets those) need [CONFIRM: service area] from the client first.

Quality gate: each location page needs real local content, such as projects for customers from that town, driving directions or time from Krzyszkowice, and a local review. Without that, don't create the page. Hard cap: 10 location pages. The template's warning level of 30 doesn't fit a single-workshop business.

## Portfolio (`/realizacje/`): replaces the per-make pages

The old site has one page per make (Audi, Buick, Cadillac, Ford, Jeep, Lincoln, Mercedes, Oldsmobile, Opel, Peugeot, Porsche, Renault, Seat, Subaru, Willys). Plan:

- Make pages with enough material (6+ photos and a story about the work) → become a `/realizacje/<marka>-<model>/` project page.
- Thin make pages → 301 to `/realizacje/` filtered or anchored by make, e.g. `/realizacje/#ford`. Don't keep 15 thin pages.
- Each project page links to the service page(s) it shows, and each service page shows its 3 best projects.

## Internal linking

```
Home ──► each service, /realizacje, /o-firmie, /kontakt
Service ──► 3 related projects, /cennik, /faq anchor, /kontakt, sibling services (max 3)
Project ──► service(s) used, other projects of same make/era
Location ──► top services, local projects, /kontakt
Blog post ──► 1 money page (service) + 1 project
Every page ──► footer: NAP, hours, phone, all services
```

- Breadcrumbs on every page below home (`BreadcrumbList` schema).
- Anchor text is the descriptive keyword ("obszycie kierownicy skórą"), never "kliknij tutaj".
- Classic cars is the hub of the heritage cluster. It links to `/pojazdy-konne/`, `/renowacja-mebli-antycznych/` and `/o-firmie/`.

## Navigation

- **Header:** Usługi (dropdown) · Realizacje · O firmie · Opinie · Kontakt · [📞 605 304 999] button
- **Mobile:** sticky bottom bar with "Zadzwoń" and "Dojazd" (Google Maps link)
- **Footer:** full NAP (exactly as in GBP), hours, landline (12) 272 23 65, service list, area served, privacy policy

## Redirect map (old → new)

URLs below are confirmed from research. **Crawl the full old site before launch** to get the rest; each per-make page needs a row.

| Old URL | New URL |
|---|---|
| `/` | `/` |
| `/o-firmie.html` | `/o-firmie/` |
| `/kontakt.html` | `/kontakt/` |
| `/struktura-cen.html` | `/cennik/` |
| `/kierownice.html` | `/uslugi/obszywanie-kierownic/` |
| `/samochody-zabytkowe-cadilac.html` | `/realizacje/cadillac-limuzyna/` |
| other per-make pages | `/realizacje/<marka>-<model>/` or `/realizacje/#<marka>` |
| `www.` host | non-www (or the reverse; choose one and redirect the other) |

## Sitemap

- One `sitemap.xml` covering the indexable pages in the hierarchy. Leave out `/polityka-prywatnosci/` (noindex is fine).
- `<lastmod>` only when content really changes.
- Submit in Google Search Console and Bing Webmaster Tools. Reference it in `robots.txt`.

## NAP: use exactly this everywhere

```
Rymarstwo – Marcin Nowak, Tapicer samochodowy
Krzyszkowice 320A, 32-445 Krzyszkowice
tel. 605 304 999 · tel. stacjonarny (12) 272 23 65
pon.–pt. 08:00–17:00, sob.–nd. nieczynne
```

Open questions to settle before content is written: email, NIP/REGON display, social links, years-in-business figure, lead-time wording, extra towns (all [CONFIRM] in `research.md`).

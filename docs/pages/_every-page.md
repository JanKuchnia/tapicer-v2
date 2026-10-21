# Every Page: Shared Requirements

## Head
- [ ] Unique `<title>` (≤ 60 chars) in the form `<Topic> – Tapicer samochodowy Kraków, Myślenice | Marcin Nowak`
- [ ] Unique meta description (≤ 155 chars) that ends with `☎ 605 304 999`
- [ ] Self-referencing canonical on the one canonical host
- [ ] `lang="pl"`, viewport meta, favicon
- [ ] Open Graph: title, description, a real photo (1200×630)
- [ ] JSON-LD: the page's own schema plus `BreadcrumbList` (all pages except home), with business references via `@id` `https://tapicer-samochodowy.pl/#business`

## Header
- [ ] Logo/name linking to `/`
- [ ] Nav: Usługi (dropdown of all 10) · Realizacje · O firmie · Opinie · Kontakt
- [ ] Call button `605 304 999` (`tel:+48605304999`), always visible

## Body
- [ ] Exactly one H1, containing the page's primary keyword
- [ ] Breadcrumbs below the header (except home)
- [ ] Original photos only, with descriptive Polish alt text, WebP/AVIF, width/height set, below-the-fold images lazy-loaded
- [ ] At least one call CTA in the content, besides header and footer

## Mobile
- [ ] Sticky bottom bar: **Zadzwoń** (tel:) · **Dojazd** (Google Maps link to the GBP listing)
- [ ] Tap targets ≥ 44px, no horizontal scroll

## Footer
- [ ] NAP exactly as in `../SITE-STRUCTURE.md` (name, address, both phones, hours)
- [ ] List of all services (links)
- [ ] Service area: Kraków, Myślenice
- [ ] Link to `/polityka-prywatnosci/`
- [ ] Current-year copyright (not 2017)
- [ ] Email, socials, NIP/REGON: **[CONFIRM]**, leave out until answered

## Copy rules
- [ ] Polish, in the client's voice: personal, proud of the craft, formal-polite
- [ ] No prices. No "szybko", "ekspresowo" or "zawsze na czas"
- [ ] Say booking ahead is needed ("terminy ustalamy z wyprzedzeniem")
- [ ] Spell it "Cadillac" (the old site's "Cadilac" is a typo)
- [ ] Don't use the "ponad 12 lat" figure; use the dates 1998 / 2004

## Performance
- [ ] LCP < 2.5 s, INP < 200 ms, CLS < 0.1 (mobile)

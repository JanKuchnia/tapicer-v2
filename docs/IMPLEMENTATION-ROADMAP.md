# Implementation Roadmap

## Phase 0: Before build (week 0)

- [ ] Client answers the [CONFIRM] items in `research.md`: email, NIP/REGON, socials, years figure, lead-time wording, extra towns, "Automotive Interiors Leather" tagline
- [ ] Crawl the old site (all `.html` URLs) to complete the redirect map in `SITE-STRUCTURE.md`
- [ ] Get GSC access for the existing domain (baseline data, keeps history)
- [ ] Collect photos into `assets/`

## Phase 1: Foundation (weeks 1–4)

- [ ] Build the site: static, HTTPS, one canonical host, mobile-first, sticky call bar
- [ ] P0 + P1 pages from `CONTENT-CALENDAR.md`
- [ ] JSON-LD: `AutoRepair` site-wide, `Service`, `BreadcrumbList`, `AboutPage`/`Person`, `ContactPage`
- [ ] `sitemap.xml`, `robots.txt`, 301 redirect map, custom 404
- [ ] GSC + Bing Webmaster, GA4 (or Plausible) with call-click event tracking
- [ ] Launch, then watch GSC Coverage / 404s daily for 2 weeks
- [ ] **Done when:** all old URLs return 301 → 200, CWV pass on mobile, every page passes the Rich Results Test

## Phase 2: Expansion (weeks 5–12)

- [ ] Claim, verify and fully fill in GBP; monthly posts
- [ ] Clean up NAP on all directories listed in `SEO-STRATEGY.md`
- [ ] Start the review-request routine after each job
- [ ] Launch `/poradnik/` at 2 pieces/month
- [ ] Remaining P2 pages; turn old make pages into project pages
- [ ] Run the competitor and SERP checks in `COMPETITOR-ANALYSIS.md`
- [ ] **Done when:** GBP verified, 10+ directory listings consistent, 4 blog posts live

## Phase 3: Scale (weeks 13–24)

- [ ] Extra location pages only if the client confirms the towns and real local content exists (cap 10)
- [ ] Links: classic-car clubs, zlot/rally organisers, restoration forums, local Myślenice/Kraków media. Offer project stories, not paid links
- [ ] Get listed on "best tapicer Kraków" roundups (GEO signal)
- [ ] Refresh service pages using GSC queries (add the questions people actually search)
- [ ] **Done when:** 5+ new referring domains, 3+ classic-car keywords in top 10

## Phase 4: Authority (months 7–12)

- [ ] Flagship case studies (long-form classic restorations with process photos, maybe video)
- [ ] Pitch the heritage story (rymarstwo → klasyki) to regional press or moto media
- [ ] Track AI citations (ask ChatGPT / Perplexity "tapicer samochodowy Kraków" monthly)
- [ ] Quarterly content refresh; prune or merge anything with no impressions after 6 months
- [ ] **Done when:** 12-month KPIs in `SEO-STRATEGY.md` are reviewed against baseline

## Dependencies

- Content depends on client photos and answers. This is the critical path.
- Redirect map depends on the full crawl of the old site.
- Review growth depends on the client actually sending the review link.

## Resources

- Developer: about 1–2 weeks for the build
- Copy: about 25 launch pages, then about 2 pieces/month
- Client: about 2 h/month for photos, review requests and approving copy

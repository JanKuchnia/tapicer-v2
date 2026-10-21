# Opinie: `/opinie/`

**Goal:** social proof, and a route to leave a Google review.
**Schema:** none for the aggregate. Google ignores self-serving `AggregateRating` on LocalBusiness, so don't add it. Individual `Review` markup is optional
**H1:** `Opinie klientów`

## Sections
1. Selected **real** reviews with name/initials, date, source (Google, Nicelocal) and a link to the source
2. Button "Wystaw opinię w Google" (GBP review short-link)
3. Link to the Google Maps profile with all reviews

## Rules
- [ ] Only reviews with permission or that are publicly visible; never invent or edit them
- [ ] Don't hide that there are mixed reviews; just curate them honestly
- [ ] Launch only once GBP has reviews (P2)

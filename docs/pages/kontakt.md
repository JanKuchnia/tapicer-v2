# Kontakt: `/kontakt/`

**Goal:** a phone call or a visit. Zero friction.
**Primary keyword:** tapicer Krzyszkowice kontakt · **Min words:** 200
**Schema:** `ContactPage` + full `AutoRepair` entity (with `geo`)
**H1:** `Kontakt`
**Redirect target for:** `/kontakt.html`

## Must include
- [ ] Big tap-to-call: **605 304 999**; landline (12) 272 23 65
- [ ] Address: Krzyszkowice 320A, 32-445 Krzyszkowice, exactly as in GBP
- [ ] Hours: pon.–pt. 08:00–17:00, sob.–nd. nieczynne
- [ ] Embedded Google Map + a "Wyznacz trasę" link
- [ ] Directions note (from Kraków / Myślenice), photo of the entrance or gate so people find it
- [ ] Short form: name, phone, vehicle, message, optional photo upload; RODO consent checkbox linking to `/polityka-prywatnosci/`
- [ ] "Terminy ustalamy z wyprzedzeniem – zadzwoń, aby zarezerwować"
- [ ] Email **[CONFIRM]**, socials **[CONFIRM]**, NIP/REGON **[CONFIRM: whether to show]**

## Tech
- Form submissions go to the client's email/SMS [CONFIRM where]; spam protection (honeypot, not a hard CAPTCHA)

# De Financiële Markt

Financieel nieuws in headliner-stijl: alle koppen op één lijst, filters op markt, bedrijf, persoon, land en onderwerp, eigen favorieten met eigen link. Een bericht is pas *bevestigd* als twee onafhankelijke redacties het melden. Geen beleggingsadvies.

Zelfde basis als [screensoccer](https://github.com/erwinvanderwacht/screensoccer). De backend (Cloudflare Worker die elk half uur feeds ophaalt, tagt en bevestigt) staat in die repo en wordt met een eigen bronnen- en entiteitenlijst hergebruikt.

## Demo

`main` deployt automatisch naar https://definancielemarkt.pages.dev (Cloudflare Pages, geen buildcommando, outputmap `public`).
Zolang er geen `/api/feed` is, toont de pagina `public/demo.json`: een momentopname van echte koppen uit NOS en NU.nl met directe artikellinks.

Eigen link: `https://definancielemarkt.pages.dev/?mijn=club:ASML,theme:rente,comp:AEX`

## Nog te doen

* Bronnenlijst: FD, IEX, De Telegraaf Financieel, RTL Z, Business Insider, Reuters, Bloomberg, CNBC, FT, Handelsblatt, Les Echos, officiële persberichten (Euronext, AFM, DNB, ECB).
* Koersen per bedrijf en index uit een data-API naast de koppen.
* Domein definancielemarkt.nl koppelen.

# Tajemství kvalitního spánku: náhled webu (v2, předprodej)

Statický one-page web (Bootstrap 5.3.3 z CDN, bez build kroku).

- `index.html`: celý web včetně stylů a skriptů
  - data 33 kartiček: proměnná `CARDS`
  - produkty a ceny: proměnná `PROD` (+ texty v sekci `#obchod`)
  - košík: Bootstrap offcanvas `#cart`, ukládá se do localStorage
- `img/`: obálka, ilustrace, ikony, kartičky (`cards/c-XX.jpg`, liché = líc, sudé = rub), ukázkové stránky

Spuštění: otevři `index.html` v prohlížeči, nebo `npx serve .`

Před spuštěním naostro:
1. Pokladnu (`#stepAddr`) napojit na platby (např. Stripe Checkout, GoPay, Comgate) nebo e-shop (Shoptet), dopravu na Zásilkovnu.
2. Ukazatel předprodeje (`#fundN`, `#fundBar`) napojit na skutečný počet objednávek. Teď jsou to ukázková data.
3. Formulář `#wlForm` napojit na e-mailovou službu (Ecomail, MailerLite…).
4. Doplnit obchodní podmínky, GDPR, reklamační řád, IČO prodávajícího, portrét autorky a termín odeslání.

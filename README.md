# The Scan Clinic: maintenance page

A static page to show while thescanclinic.co.uk is down or under maintenance. It tells visitors the site is temporarily unavailable and gives them the phone number, WhatsApp and email.

It's served by GitHub Pages from the root of the `main` branch.

## Files

- `index.html`: the page. All CSS is inline; the fonts (Fraunces and Inter) load from Google Fonts.
- `404.html`: a copy of `index.html`, so any path on the Pages site (for example `/ultrasound-scan-prices/`) shows the same message.
- `assets/`: logo and clinic photo, kept here so the page doesn't depend on the main website being up.
- `.nojekyll`: tells GitHub Pages to serve the files as they are, without running Jekyll.

## Editing

Change `index.html`, then copy it over `404.html` so the two stay the same:

```sh
cp index.html 404.html
```

Contact details used on the page:

- Phone: 020 3904 7706 (`tel:+442039047706`)
- WhatsApp: 07584 426428 (`https://wa.me/447584426428`)
- Email: customercare@thescanclinic.co.uk

## Using it during an outage

The page is always live at the GitHub Pages address. To show it on the real domain during an outage, either point the domain's DNS at GitHub Pages and add the domain under **Settings → Pages → Custom domain**, or redirect visitors to the Pages address from the host or CDN. Undo the change when the site is back.

The page has `noindex` set so search engines don't index it in place of the real site.

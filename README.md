# WonderBox website

Static website for WonderBox, a student-run nonprofit that delivers free care packages to hospitalized children.

Live at https://agentknightsofficial.github.io/Wonderbox-Website/

## Files

- `index.html` is the home page: the interactive box in the hero and every section below. Items inside the box jump to those sections.
- `team.html` is the team page.
- `styles.css` holds the styling for both pages.
- `about.html` redirects old links to the team page.
- `wonderbox-logo.png` is the logo.
- `img/` holds photos. `img/share-banner.png` is the preview image shown when the link is shared.

No build step is needed. Open `index.html` in a browser to preview.

## Common edits

These settings are at the top of the `<script>` near the end of `index.html`.

- **Donate buttons:** they deliberately go nowhere right now. To link them again, set `a.href` in `wireDonate` in `index.html` and in the inline script of `team.html`.
- **Photos:** drop the image into `img/`, then add a line to `PHOTOS`, for example
  `{ src: "img/shopping-trip.jpg", alt: "The team shopping for toys" },`
  (Photos show without captions; `alt` is only for screen readers.)
  New photos appear in the Chapter 1 gallery.
- **Donation page screenshot:** put it in `img/` and set `DONATION_SHOT = "img/donation-page.png"`.

Text lives in the HTML:

- Stats: the `bento` tiles in `index.html` (the `$3,500` is `data-count="3500"`).
- Box contents by age: the `age-panel` sections.
- Team bios and photos: the `slip` cards in `team.html`.
- Contact email: search for `wonderboxnpo@gmail.com`.

## Publishing

GitHub Pages serves the `main` branch root. Commit and push, and the live site updates in a minute or two.

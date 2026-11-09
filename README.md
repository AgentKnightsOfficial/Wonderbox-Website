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

All three settings are at the top of the `<script>` near the end of `index.html`.

- **Donate link:** change `DONATE_URL`.
- **Photos:** drop the image into `img/`, then add a line to `PHOTOS`, for example
  `{ src: "img/shopping-trip.jpg", caption: "our first shopping run", alt: "The team shopping for toys" },`
  New photos appear in the Chapter 1 gallery.
- **Donation page screenshot:** put it in `img/` and set `DONATION_SHOT = "img/donation-page.png"`.

Text lives in the HTML:

- Stats: the `bento` tiles in `index.html` (the `$3,500` is `data-count="3500"`).
- Box contents by age: the `age-panel` sections.
- Team bios and photos: the `slip` cards in `team.html`.
- Contact email: search for `wonderboxnpo@gmail.com`.

## Publishing

GitHub Pages serves the `main` branch root. Commit and push, and the live site updates in a minute or two.

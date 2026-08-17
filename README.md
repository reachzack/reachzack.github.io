# Academic homepage template

Same layout, colors, fonts, and card style as the reference site
(javyduck.github.io, which itself is forked from jonbarron.github.io):
warm parchment background, serif display headings, maroon accents,
bordered "card" boxes for experience/publications, bio on the left
with a circular photo + quote on the right.

## Files
- `index.html` — page content (edit the bracketed `[...]` placeholders)
- `stylesheet.css` — all styling (colors/fonts live in the `:root` block up top)
- `images/logo_placeholder.svg` — gray placeholder box used for employer logos
- `images/` — put your real photo, employer logos, and publication images/GIFs here

## What's a placeholder right now
- `images/profile_circle.jpg`, `images/profile_full.jpg` — your headshot (not included yet)
- `images/logo_placeholder.svg` — swap for real employer/university logos as you get them
- Each publication has a dashed-border **"Image / GIF placeholder"** box on the left.
  When you have a figure or GIF ready, replace:
  ```html
  <div class="pub-placeholder"><span>Image / GIF<br>placeholder</span></div>
  ```
  with:
  ```html
  <img class="pub-image" src="images/your-file.gif" alt="Short description">
  ```

## Adding more entries
- Copy an `.intern-box` block to add another job/appointment.
- Copy a `.pub-box` block (it includes its own `.pub-media` placeholder) to add another publication.
- Add a new `<div class="pub-year">2024</div>` line whenever the year changes.

## Optional background texture
The reference site uses a faint SVG doodle behind the text (`images/math-doodles.svg`).
It's left out here since it's a personal asset — drop your own SVG/PNG into `images/background.svg`
and uncomment the `background-image` lines near the top of `stylesheet.css` if you want that effect.

## Viewing locally
Just open `index.html` in a browser — no build step needed. To publish, push this folder
to a GitHub repo named `<your-username>.github.io` and enable GitHub Pages.

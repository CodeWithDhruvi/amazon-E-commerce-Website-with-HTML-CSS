# Amazon Home Page — HTML & CSS

**Project type:** Static front-end (HTML + CSS)

**Purpose:**
A simple, static replica of an Amazon-style home page built using only `index.html` and `style.css`. This project demonstrates layout, navigation/header, hero, product category cards, and footer sections using plain HTML and CSS. Font Awesome is used for icons.

---

## Files in this project

* `index.html` — Main HTML document (header, search, panel, hero, shop sections, footer).
* `style.css` — All styling for the page (layout, colors, spacing, responsive helpers).
* `amazon_logo.png` — (optional) logo image used in header/footer. Place this in the same folder.
* `hero_image.jpg`, `box1_image.jpg` ... `box8_image.jpg` — placeholder images for hero and category boxes. Place these in the same folder.

> **Note:** If you don't have the image files, the page will still load but the areas will be blank or fall back to the default background. Use any JPG/PNG images and name them as above, or update the `index.html` inline `background-image` URLs to match your image filenames.

---

## How to view (run) the project

1. Make sure `index.html` and `style.css` are in the same folder.
2. Put the optional images (`amazon_logo.png`, `hero_image.jpg`, `box*_image.jpg`) in the same folder.
3. Open `index.html` in any modern browser (Chrome, Firefox, Edge, Safari). Double-click the file or right-click → Open with → *Browser*.

No server, build tools, or installations are necessary — this is pure static HTML/CSS.

---

## Edit and customization tips

* **Change placeholder text / headings:** Edit the headings and paragraphs directly inside `index.html`.
* **Swap images:** Replace the `box*_image.jpg` and `hero_image.jpg` files or change the `background-image` URL values in `index.html`.
* **Logo:** Replace `amazon_logo.png` with your own logo and keep the same filename or update the CSS `background-image` value.
* **Font Awesome icons:** The project includes Font Awesome via CDN. To use other icons, update the `<i class="...">` class names. CDN link is already in `index.html`.
* **Make responsive:** The layout currently uses fixed widths and percentages. To make the site responsive, add media queries to `style.css` and adjust `.shop-section .box` width (for example, change `width: 23%` for smaller screens).

---

## Small fixes & improvements you might want

* Fix typo `Eelectronics` → `Electronics` in `index.html`.
* In `style.css`, replace `border: border-box;` (invalid) with `box-sizing: border-box;` at the top: e.g.

  ```css
  * { box-sizing: border-box; }
  ```
* Use semantic elements where appropriate (e.g., `<nav>`, `<main>`, `<section>`) to improve accessibility.
* Add `alt` attributes to any inline `<img>` tags (if you convert background images to `<img>` elements) for accessibility.
* Add `:focus` styles for keyboard users and `aria-*` attributes where helpful (e.g., `aria-label` on search input).
* Consider using `flex-wrap` and percentage max widths or CSS Grid to make the card layout adapt to small screens.

---

## Git basics (optional) — quick start

If you want to put this project in a git repository locally:

```bash
# from project folder
git init
git add index.html style.css amazon_logo.png hero_image.jpg box1_image.jpg
git commit -m "Initial commit: Amazon home page HTML & CSS"
```

To push to GitHub (create a repo on GitHub first):

```bash
git remote add origin https://github.com/<your-username>/<repo-name>.git
git branch -M main
git push -u origin main
```

---

## Credits

* Icons: Font Awesome (CDN included in `index.html`).
* Images: Use royalty-free images from Unsplash / Pexels / Pixabay if you need replacements.

---

## License

This project is released under the **MIT License**. Use freely, attribute if you like.

---

If you'd like, I can:

* Create a responsive variant (`@media` queries) for mobile screens.
* Convert the category boxes to use `<img>` tags with `alt` text.
* Generate a short changelog or TODO file for improvements.

Tell me which of the above you'd like next and I will add it.

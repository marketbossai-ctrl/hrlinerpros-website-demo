# Hampton Roads Liner Pros — Website

This is a static HTML website, built for speed and local SEO. There is no CMS,
no database, and no build step — every page is a plain HTML file. That means
**anyone can edit it** without a developer or an agency.

## How to Make Common Edits

**Change the phone number** — it appears in:
- `index.html` (header + hero)
- `contact.html`
- Every page's header (in the top bar)

Search the whole site for the old number and replace it. On GitHub, click the
file, click the pencil icon ✏️, edit, then "Commit changes".

**Change a paragraph** — open the page, find the text, edit it. Done.

**Add a new service** — add a new folder under `services/` with an `index.html`
(copy an existing service page and change the text), then add it to the list in
`services/index.html` and `index.html`.

**Change the colors** — open `css/style.css` and edit the `:root` variables at
the top. `--primary` is the main color, `--accent` is the button color.

**Change the logo** — replace the image file in `img/` with your new logo.

## How It Was Built

Generated with Market Boss AI's local SEO site generator. Every page has:
- Unique title tag and meta description
- JSON-LD structured data (LocalBusiness, Service, FAQ, Breadcrumbs)
- Exactly one H1, with proper H2/H3 hierarchy
- Semantic HTML5 and mobile-responsive CSS

## Structure

```
index.html          → Homepage
about.html          → About page
contact.html        → Contact (with form)
reviews.html        → Customer reviews
services/           → One page per service
service-areas/      → One page per city served
css/style.css       → Single stylesheet (edit colors here)
img/                → Images
sitemap.xml         → Auto-generated sitemap
robots.txt          → Crawler instructions
```

## Publishing

This site is hosted on GitHub Pages. Push to the `main` branch and it goes live
within a minute or two. To use a custom domain, add a `CNAME` file with the
domain name and configure DNS.

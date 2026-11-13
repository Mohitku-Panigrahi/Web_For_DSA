# Web For DSA

A curated, interactive directory of websites for learning data structures and algorithms, preparing for coding interviews, practising competitive programming, and building AI/ML and web-development skills.

The site helps you choose a focused practice stack instead of searching through a long, unstructured list of resources.

## Features

- Browse 26 coding-practice platforms grouped into five categories:
  - DSA and interview preparation
  - Competitive programming and contests
  - Fundamentals and language practice
  - Projects and interactive challenges
  - AI/ML and data
- Search by platform, skill, language, topic, or use case.
- Filter by category, pricing, and experience level.
- Save favorite platforms in the browser with the star button.
- View each platform's description, pricing, level, and recommended use.
- Open external resources in a new tab.
- Responsive layout for desktop and mobile screens.
- Reduced-motion and print-friendly styling.

## Getting started

This is a static HTML project, so no package installation or build step is required.

### Run locally

1. Clone the repository:

   ```bash
   git clone https://github.com/Mohitku-Panigrahi/Web_For_DSA.git
   cd Web_For_DSA
   ```

2. Open `index.html` in a browser.

   For a local web server, run:

   ```bash
   python3 -m http.server 8000
   ```

   Then visit <http://localhost:8000>.

## Project structure

```text
.
├── index.html   # Complete static site: markup, styles, platform data, and JavaScript
└── README.md
```

## How it works

- Platform information is stored in the `S` array in `index.html`.
- Categories and their descriptions are defined in `CATS`.
- Search and filters update the rendered platform cards without a page reload.
- Favorites are stored in the browser's `localStorage` under the `cp_saved` key.
- External links use `target="_blank"` with `rel="noopener noreferrer"`.

## Adding or updating a platform

Edit the `S` array in `index.html` and add or update an entry with these fields:

```js
{
  c: "dsa",                  // Category key from CATS
  n: "Platform name",
  u: "https://example.com/",
  tag: "Short label",
  d: "Platform description.",
  best: "What it is best for",
  l: "B",                    // B: Beginner, I: Intermediate, A: Advanced
  p: "Free",                 // Free, Freemium, or Paid
  k: "searchable keywords"
}
```

Keep descriptions concise and verify external URLs before submitting changes.

## Contributing

1. Create a branch for your change.
2. Update `index.html` and/or `README.md`.
3. Open `index.html` in a browser and verify search, filters, favorites, and external links.
4. Submit a pull request describing the change.

## License

No license has been specified for this repository yet. Contact the repository owner before redistributing or reusing the code.

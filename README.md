# Yuki Cordero Portfolio — Production Package

This package contains the production-ready branded portfolio website for Yuki Cordero. The site is a static GitHub Pages-ready build and opens from the root `index.html` file.

## Package structure

```text
/
├── index.html
├── styles.css
├── script.js
├── README.md
├── .nojekyll
├── site.webmanifest
├── assets/
│   ├── images/
│   ├── logos/
│   ├── favicons/
│   └── brand/
├── css/
│   └── yc-brand-tokens-expanded.css
└── docs/
    ├── portfolio-copy-and-structure.md
    ├── logo-usage-guide.md
    └── launch-qa-checklist.md
```

## Visual direction preserved

The current premium YC identity has been preserved: dark navy background, gold accent system, cream text, modern portfolio layout, and professional AI Automation / Tech VA positioning. This cleanup reorganizes files and improves production readiness without redesigning the site from scratch.

## Required Before Launch

The final GitHub Pages URL was not provided, so the package intentionally keeps URL placeholders. Do not invent the deployment URL. After the repository is created and GitHub Pages is enabled, replace every placeholder with the final public URL.

Current placeholder format:

```text
https://YOUR-GITHUB-USERNAME.github.io/YOUR-REPOSITORY-NAME/
```

Update the following file and fields after the final URL is known:

### `index.html`

- `<link rel="canonical">` href
- `<meta property="og:image">` content
- `<meta name="twitter:image">` content
- JSON-LD `Person.@id`
- JSON-LD `Person.url`
- JSON-LD `ProfessionalService.@id`
- JSON-LD `ProfessionalService.url`
- JSON-LD `ProfessionalService.provider.@id`
- JSON-LD `WebSite.@id`
- JSON-LD `WebSite.url`

The social preview fields should use the absolute deployed image URL, for example:

```text
https://YOUR-GITHUB-USERNAME.github.io/YOUR-REPOSITORY-NAME/assets/images/social-preview.png
```

### `site.webmanifest`

- Optional after deployment: change `start_url` and `scope` from relative paths to the final public URL if a fully absolute manifest is preferred. The current relative configuration is safe for GitHub Pages project sites.

### External service/contact fields to confirm

- Calendly URL
- LinkedIn URL
- Email address and mailto subject
- Loom demo links
- GitHub repository links for both case studies
- Published rate and availability details

## Logo and favicon assets

Production logo files live in `assets/logos/`:

- `yc-logo-primary-light.svg`
- `yc-logo-reversed-dark.svg`
- `yc-icon-standalone.svg`
- `yc-logo-monochrome.svg`

Favicon assets live in `assets/favicons/`:

- `yc-favicon.svg`
- `favicon-16x16.png`
- `favicon-32x32.png`
- `favicon-48x48.png`
- `favicon-180x180.png`
- `favicon-512x512.png`
- `apple-touch-icon.png`
- `favicon.ico`

The SVG logo files are path-based for production consistency. If they are edited in a design tool later, convert any live text back to paths before export.

## Supporting documents

- `docs/logo-usage-guide.md` explains how to use each logo and favicon file.
- `docs/portfolio-copy-and-structure.md` records the final copy direction and recommended homepage structure.
- `docs/launch-qa-checklist.md` lists final checks before GitHub Pages deployment.

## Local preview

Open `index.html` directly in a browser, or run a small local server from the package root:

```bash
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## GitHub Pages deployment

1. Create a GitHub repository.
2. Upload the full contents of this package root, not the ZIP itself.
3. Go to **Settings → Pages**.
4. Choose **Deploy from a branch**.
5. Select the `main` branch and `/root` folder.
6. Save the Pages settings.
7. After GitHub publishes the site, update the placeholders listed in **Required Before Launch**.
8. Run the checklist in `docs/launch-qa-checklist.md`.

## Final static QA performed in this cleanup

- Root `index.html` remains the site entry point.
- Local asset paths referenced by HTML and manifest were checked.
- Internal anchor targets were checked.
- External new-tab links were checked for `rel="noopener noreferrer"`.
- Image elements were checked for `alt` attributes.
- JavaScript was checked for syntax errors.
- JSON-LD was parsed as valid JSON.
- Temporary and duplicate root-level brand files from the earlier package were removed or consolidated into the cleaner structure.

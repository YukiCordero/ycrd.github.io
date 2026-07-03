# Launch QA Checklist

Use this checklist immediately before publishing the Yuki Cordero portfolio site and again after the GitHub Pages URL is live.

## Placeholder replacement checklist

- Replace every `YOUR-GITHUB-USERNAME` placeholder in `index.html`.
- Replace every `YOUR-REPOSITORY-NAME` placeholder in `index.html`.
- Confirm the canonical URL exactly matches the final GitHub Pages URL.
- Confirm Open Graph and Twitter image URLs use the absolute deployed path to `assets/images/social-preview.png`.
- Confirm JSON-LD `@id` and `url` fields use the final deployed URL.
- Confirm Calendly, LinkedIn, email, Loom, and GitHub project links are final.

## SEO metadata checklist

- Page title is specific and includes Yuki Cordero plus the AI Automation / Tech VA positioning.
- Meta description is clear, concise, and outcome-oriented.
- Canonical URL uses the final published URL.
- JSON-LD parses as valid JSON.
- JSON-LD fields match the visible page content.
- No placeholder deployment URLs remain after launch.

## Social preview checklist

- `assets/images/social-preview.png` exists.
- Preview image is 1200×630.
- Open Graph image URL is absolute after deployment.
- Twitter/X image URL is absolute after deployment.
- Image alt text describes the portfolio preview accurately.
- Test the published URL in social preview/debug tools after deployment.

## Accessibility checklist

- Every image has an `alt` attribute.
- Decorative images either use empty alt text with appropriate surrounding labels or concise descriptive alt text.
- The skip link points to `#main`.
- Interactive elements have visible focus states.
- Mobile navigation can be opened, closed, and dismissed with keyboard controls.
- Link text is meaningful without relying only on surrounding context.
- Color contrast remains readable on dark navy, gold, cream, and muted text surfaces.
- Reduced-motion preferences are respected.
- Page remains readable with JavaScript disabled.

## Mobile responsiveness checklist

- Test at 320px, 375px, 414px, 768px, 1024px, and desktop widths.
- Confirm the header does not overflow before the mobile menu breakpoint.
- Confirm CTAs remain tappable and at least 44px high.
- Confirm project screenshots scale without horizontal scrolling.
- Confirm tool cards wrap cleanly.
- Confirm hero portrait badges do not cover important image content.
- Confirm anchor jumps are not hidden behind the sticky header.

## Link testing checklist

- Test all internal navigation anchors: Home, Services, Projects, Process, Results, FAQ, Contact, and Back to top.
- Test Calendly workflow review links.
- Test email mailto links.
- Test LinkedIn link.
- Test Loom demo links.
- Test GitHub repository links.
- Test full workflow screenshot links.
- Confirm every new-tab external link uses `target="_blank"` and `rel="noopener noreferrer"`.

## Performance checklist

- Keep the hero profile image preloaded and prioritized.
- Keep below-the-fold images lazy-loaded.
- Confirm images have explicit width and height attributes.
- Confirm no unused temporary images or duplicate root-level assets remain.
- Confirm JavaScript runs without console syntax errors.
- Confirm CSS loads from the root `styles.css`.
- Optional: minify images or CSS only after the final visual approval.

## Final GitHub Pages deployment checklist

- Upload the package contents to the repository root.
- Keep `.nojekyll` in the root.
- Confirm `index.html` is in the root.
- Enable Pages from the `main` branch and `/root` folder.
- Open the live URL after deployment.
- Replace placeholder deployment URLs in `index.html`.
- Commit and push the placeholder replacements.
- Re-open the live URL and verify metadata, images, links, and mobile layout.
- Test social preview after the final URL is live.

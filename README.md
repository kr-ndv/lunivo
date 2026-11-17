# Vayanvesha

**Discover beyond boundaries.** An independent directory for educational websites, digital libraries, research platforms and learning resources from India and around the world.

## Product

A static, dependency-light website built with vanilla HTML, CSS and JavaScript.

- Responsive directory with dark and light themes
- Search across resource names, descriptions and catalogue metadata
- Category, subject, region, education-level and access filters
- Alphabetical, featured and recently-added sorting
- Seven curated collections, including a dedicated India learning shelf
- Browser-only bookmarks with no account or cross-device sync
- Resource detail dialog with source, access and review information
- Keyboard-accessible dialogs, focus return, reduced-motion support and visible focus
- Empty, loading and catalogue-error states
- No backend, build step or runtime package required

## Run locally

Open `index.html` in a modern browser. The site uses system font stacks to avoid third-party font requests and provide fast, resilient rendering.

## Deploy

Published with GitHub Pages from the `main` branch at the repository root. The repository is currently named `lunivo`, so the temporary project URL remains https://kr-ndv.github.io/lunivo/ until a custom domain and repository URL migration are configured.

## Catalogue and editorial policy

The catalogue retains the original CBSE Library external-link starting list and records additions from official institutional or service sources. See `SOURCES.md` for the source register and legacy review notes.

Vayanvesha is independent and is not affiliated with CBSE, NCERT, the Ministry of Education or any listed service. Resource descriptions are editorial summaries. A source review date means the reference was checked during curation. It is not a live uptime check or a guarantee of availability, eligibility, licensing or free access. Access conditions may vary by item, account, location and institution.

Legacy or ambiguous entries are marked **Needs review** in the catalogue. Do not treat a historical listing as evidence that a service is still active or that a current destination is its successor.

## Security and performance

- Static hosting; no server-side application, database, login or secrets.
- No third-party JavaScript, analytics, trackers or remotely hosted fonts.
- A document-level Content Security Policy and strict referrer policy are included.
- GitHub Pages does not provide arbitrary response-header configuration. On a custom domain/CDN, configure HSTS, frame protection, MIME-sniffing protection, Permissions Policy and a production CSP as HTTP response headers.
- External links opened in new tabs use `rel="noopener noreferrer"`.
- Browser storage contains only local bookmarks and theme preference.
- No runtime dependencies to patch.

## Contributing

Use the GitHub Issues links in the site footer to suggest a resource or report a broken destination. Include the official resource URL and a supporting source where possible. There is no in-site submission backend or moderation dashboard.

## Editorial launch checklist

- Review the legacy records still marked **Needs review**.
- Recheck destination availability, access descriptions and usage terms periodically.
- Test current desktop and mobile browsers, keyboard-only use, screen-reader labels and both themes.
- Check all external links after deployment. Browser-only bookmarks are stored on the visitor's device and do not sync.

## Brand

Vayanvesha is a coined blend inspired by Malayalam `vayana` (reading) and Sanskrit `anvesha` (inquiry or exploration). The identity uses the Open Book + Discovery mark and the olive, cream, amber and terracotta palette. Reusable assets are in `assets/vayanvesha-*`; the favicon and app manifest use the same mark.

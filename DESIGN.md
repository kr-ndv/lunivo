# Vayanvesha design direction

## Product identity

Vayanvesha is an independent, global directory of educational websites, digital libraries, research platforms and learning resources. Indian resources form a substantial collection within the wider directory.

The name is a coined blend inspired by Malayalam `vayana` (reading) and Sanskrit `anvesha` (inquiry or exploration). It is a brand construction, not a traditional dictionary word.

The primary audiences are students, educators, researchers and self-directed learners. The interface should help visitors judge what a resource is, who it serves, what it covers and what access conditions to expect before they leave Vayanvesha.

## Brand character

The redesigned Open Book + Discovery mark combines an open book with a search motif and a small spark. It represents reading as a starting point for inquiry, discovery and wider learning. Keep the mark's proportions and palette consistent across the website, favicon, app icon and social artwork.

## Palette

| Colour | Hex | Role |
|---|---|---|
| Deep olive | `#283618` | Primary dark background |
| Olive | `#606c38` | Book page and secondary surfaces |
| Warm cream | `#fefae0` | Light background and contrast |
| Amber | `#dda15e` | Discovery detail and highlight |
| Terracotta | `#bc6c25` | Secondary accent |

Remote Google Fonts have been removed in favour of system font stacks to remove third-party font requests and reduce render-blocking network dependencies. Light and dark themes remain first-class appearances.

## Interface decisions

- The directory uses cards because each resource needs a consistent name, type, short description, category, region, access label and set of actions.
- Search and filters sit above the catalogue because they are the primary task. Subject, region, level and access filters can be combined.
- Collections are links that apply known resource ID sets. They do not imply ranking or endorsement.
- Saved resources use browser storage only. There is no account or cross-device synchronisation.
- Resource detail dialogs expose type, subjects, level, region, access, source and review status before the visitor opens the external site.
- The recent-additions section is derived from catalogue dates. It is not an activity feed or popularity ranking.

## Content and trust

Vayanvesha is independent and is not affiliated with CBSE, NCERT, a ministry, university, publisher or any listed service. Each resource entry is an editorial directory record. The date shown as a source review date means the reference was checked during curation; it is not a live uptime test or a guarantee that every item is free, reusable or accessible.

Use clear access descriptions such as `Free search; full text varies`, `Open access books`, or `Mixed access`. Copyright and licensing conditions may vary by item and country. Mark legacy or ambiguous destinations as needing review instead of making a confident claim.

Never invent testimonials, user counts, rankings, popularity, uptime, accessibility certification or performance scores. A resource suggestion or broken-link report currently goes to GitHub Issues; it is not an in-site submission service.

## Implementation, security and performance

The project is a static site using vanilla HTML, CSS and JavaScript. Keep it dependency-light and maintainable. No backend, account system, runtime package or third-party JavaScript is required. Remote web fonts have been removed in favour of system fonts.

The HTML includes a document-level Content Security Policy and a strict referrer policy. GitHub Pages does not support arbitrary HTTP response headers from repository files. If the site later moves behind a configurable CDN or hosting provider, configure response headers there: HSTS, X-Content-Type-Options, frame protection, a Permissions Policy and a production CSP. Do not claim these headers are active on GitHub Pages unless verified at the response level.

## Brand assets

- `assets/vayanvesha-mark.svg`: compact mark.
- `assets/vayanvesha-logo.svg`: horizontal wordmark.
- `assets/vayanvesha-app-icon.svg`: scalable app icon.
- `assets/vayanvesha-social-preview.svg`: 1200 × 630 editable social artwork.
- `favicon.svg`: browser icon.
- `site.webmanifest`: install metadata and SVG app icon.

The social artwork should also be exported as a 1200 × 630 PNG and used as the Open Graph image once the raster file is committed. The static site does not include a service worker or offline functionality.

# Lunivo design direction

## Product identity

Lunivo is an independent, global directory of educational websites, digital libraries, research platforms and learning resources. Indian resources form a substantial collection within the wider directory.

The primary audiences are students, educators, researchers and self-directed learners. The interface should help visitors judge what a resource is, who it serves, what it covers and what access conditions to expect before they leave Lunivo.

## Brand character

The Open Page mark represents an open book and the act of finding a new path into knowledge. Keep the mark simple and recognisable at small sizes. The wordmark uses lowercase `lunivo` with a quiet teal accent.

The palette comes from the existing identity: deep green surfaces, warm off-white text, teal and mint accents. Light and dark themes are both first-class appearances. Use the accent for selection, important actions and links, not as decoration on every element.

Space Grotesk is the display typeface for headings and brand text. Inter is the body typeface for clear reading. System sans-serif fallbacks keep content legible when remote fonts are unavailable.

## Design read

Reading this as a content-first global educational directory for students, educators, researchers and self-directed learners, in Lunivo's Open Page visual language.

- **ENERGY 2:** calm and editorial, with a little character in the mark, typography and active states.
- **RHYTHM 3:** section composition changes with the task. The hero introduces search, categories provide a compact index, collections explain pathways, the directory is a working catalogue, and recent additions are a short list.
- **MOTION 1:** no entrance choreography or automatic movement. Use restrained hover, pressed and focus feedback. Respect `prefers-reduced-motion`.

## Interface decisions

- The directory uses cards because each resource needs a consistent name, type, short description, category, region, access label and set of actions.
- Search and filters sit above the catalogue because they are the primary task. Subject, region, level and access filters can be combined.
- Collections are links that apply known resource ID sets. They do not imply ranking or endorsement.
- Saved resources use browser storage only. There is no account or cross-device synchronisation.
- Resource detail dialogs expose type, subjects, level, region, access, source and review status before the visitor opens the external site.
- The recent-additions section is derived from catalogue dates. It is not an activity feed or popularity ranking.

## Content and trust

Lunivo is independent and is not affiliated with CBSE, NCERT, a ministry, university, publisher or any listed service. Each resource entry is an editorial directory record. The date shown as a source review date means the reference was checked during curation; it is not a live uptime test or a guarantee that every item is free, reusable or accessible.

Use clear access descriptions such as `Free search; full text varies`, `Open access books`, or `Mixed access`. Copyright and licensing conditions may vary by item and country. Mark legacy or ambiguous destinations as needing review instead of making a confident claim.

Never invent testimonials, user counts, rankings, popularity, uptime, accessibility certification or performance scores. A resource suggestion or broken-link report currently goes to GitHub Issues; it is not an in-site submission service.

## Implementation constraints

The project is a static site using vanilla HTML, CSS and JavaScript. Keep it dependency-light and maintainable. Do not add a backend, account system or framework without an explicit product decision. Ensure every control has a real action, both themes remain readable, and keyboard and mobile use remain supported.


## Brand identity — Palette 2

The current identity uses the Open Page mark: an open book with a warm bookmark, representing discovery and access to knowledge. Keep the mark's proportions and colours consistent across the site, documentation and social profiles.

| Colour | Hex | Role |
|---|---|---|
| Deep olive | `#283618` | Primary dark background and wordmark |
| Olive | `#606c38` | Mark/page accent and secondary surfaces |
| Warm cream | `#fefae0` | Light background and contrast |
| Amber | `#dda15e` | Primary highlight and page spine |
| Terracotta | `#bc6c25` | Bookmark and secondary accent |

Use the cream mark on deep olive backgrounds; use the deep-olive wordmark on cream backgrounds. Avoid placing the mark on busy imagery or recolouring individual parts outside this palette. The reusable vectors are `assets/lunivo-mark.svg` and `assets/lunivo-logo.svg`.


## Brand asset extensions

- `assets/lunivo-app-icon.svg`: square 512 × 512 app icon with a rounded deep-olive tile.
- `assets/lunivo-social-preview.svg`: 1200 × 630 social-sharing composition.
- `site.webmanifest`: lightweight install metadata and SVG icon reference.

The social preview is supplied as SVG source for easy editing and scaling. Some social platforms do not accept SVG as an Open Graph image; export a 1200 × 630 PNG for broad compatibility before using it as `og:image`. The static site does not add service-worker or offline functionality.

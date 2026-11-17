<div align="center">
  <img src="assets/vayanvesha-social-preview.svg" alt="Vayanvesha — Discover beyond boundaries. An open directory for learning, research and discovery." width="100%">
  <p><strong>Discover beyond boundaries.</strong></p>
  <p>An independent directory of educational websites, digital libraries, research platforms and learning resources from India and around the world.</p>
  <p>
    <a href="https://kr-ndv.github.io/lunivo/">Visit the website</a> ·
    <a href="https://github.com/kr-ndv/lunivo/issues/new?title=Suggest%20a%20resource">Suggest a resource</a> ·
    <a href="https://github.com/kr-ndv/lunivo/issues/new?title=Report%20a%20broken%20link">Report a problem</a>
  </p>
</div>

---

## About the project

**Vayanvesha** is a curated starting point for discovering learning and research resources. It brings together educational platforms, digital libraries, open course materials, scholarly discovery tools and cultural collections in one searchable directory.

The directory includes resources from India and international providers. It is intended for students, educators, researchers and curious self-directed learners.

Vayanvesha is an **independent directory**, not a content host, school, university, publisher, accreditation body or government service. It helps visitors find third-party resources; visitors use those resources under each provider's own terms.

## Explore the directory

The current catalogue contains **48 resource records**. Browse the directory by:

- **Category** — libraries, research, science, courses and other resource types.
- **Subject** — narrow results by the topics a resource covers.
- **Region** — distinguish India-focused resources from global services.
- **Education level** — find resources aimed at different stages of learning.
- **Access** — compare the catalogue's editorial access descriptions.
- **Search and sort** — search names and descriptions, or sort alphabetically, by featured status and recent additions.

You can also start from seven curated pathways:

| Collection | What it brings together |
|---|---|
| India learning shelf | Indian school resources, national learning platforms, libraries and academic initiatives |
| Open libraries | Books, textbooks, cultural collections and digital archives |
| Research starting points | Scholarly discovery, journals, theses and subject databases |
| Science and computing | Laboratory learning, technical courses and research tools |
| Humanities and culture | History, literature, archives, art and social sciences |
| School learning | School education, open schooling and learning materials |
| Open courses | University course materials and self-paced learning |

Collections are navigation aids, not rankings, endorsements or guarantees of quality.

## How to use it

1. Open the [Vayanvesha website](https://kr-ndv.github.io/lunivo/).
2. Search for a platform, subject or topic, or browse by category.
3. Combine filters to narrow the results.
4. Open a resource's details to review its description, subjects, region, access note and source information.
5. Visit the provider's website and check its current terms before relying on or reusing its material.

You can save resources in your browser. Saved items are stored locally on that browser and device; they do not create an account, sync between devices or follow you to another browser.

## Transparency and editorial standards

We want the directory to be useful without implying more certainty than we have.

### What a listing means

A listing is an editorial directory record. It is not a partnership, endorsement, ranking, certification or guarantee that the provider is active, safe, free or suitable for a particular purpose.

### Sources and review dates

We use official provider websites and institutional resource lists as starting points where possible. The source register and review notes are maintained in [SOURCES.md](SOURCES.md).

A **source review date** means that a reference was checked during curation. It does **not** mean that the destination was continuously monitored, that every link was successfully tested for every visitor, or that its content and access conditions remain unchanged.

### Access labels are summaries

Terms such as *Free*, *Open access*, *Mixed access* or *Free search; full text varies* are concise editorial descriptions, not legal determinations. Access may depend on the individual item, account, institution, location or subscription. Always read the provider's current terms and the rights statement for the specific item you want to use.

### Records needing review

Some older directory entries have ambiguous names, historical destinations or unconfirmed successor services. These are marked **Needs review** rather than presented as verified current services. The current review notes identify **seven legacy records** that still need manual verification. See [SOURCES.md](SOURCES.md) for the names and context.

### Independence and affiliation

Vayanvesha is not affiliated with or endorsed by CBSE, NCERT, India's Ministry of Education, any university, publisher, government body or any listed third-party service. Names and logos of third-party providers remain the property of their respective owners.

## Privacy, security and technical design

Vayanvesha is deliberately simple and static.

| Area | Current implementation |
|---|---|
| Application | Vanilla HTML, CSS and JavaScript |
| Hosting | GitHub Pages |
| Backend / database | None |
| Accounts / sign-in | None |
| Analytics / advertising | No first-party analytics or advertising code is included |
| Third-party JavaScript | None |
| Remote fonts | Removed; system font stacks are used |
| Saved resources | Browser-local storage; no account or cross-device sync |
| Theme preference | Stored locally in the browser |
| Offline support | No service worker or guaranteed offline mode |
| Data submission | Suggestions and broken-link reports open GitHub Issues; there is no in-site submission backend |

### Security notes

- The page includes a document-level Content Security Policy and a strict referrer policy.
- External links opened in new tabs use `rel="noopener noreferrer"`.
- The site has no server-side application, database credentials or user account system.
- GitHub Pages does not let this repository configure arbitrary HTTP response headers. A meta policy is not a substitute for response headers.
- If a custom domain is later placed behind a CDN or hosting layer that supports headers, configure and verify appropriate headers there, including HSTS, `X-Content-Type-Options`, frame protection, Permissions Policy and a carefully tested Content Security Policy.
- No security audit or penetration test is claimed. Please report suspected security issues through the repository's GitHub security reporting facilities, if enabled, or contact the maintainer privately rather than posting exploitable details publicly.

### Performance notes

The site has no build step or runtime package dependencies. Remote font requests were removed to reduce external requests and avoid waiting on font services. These choices reduce complexity, but they are not a published performance score. No Lighthouse, Core Web Vitals or independent load-test result is claimed in this README.

## Technology and repository layout

This is a static site. The directory data and client-side behaviour are maintained in `index.html`; there is no package manager or compilation step.

| Path | Purpose |
|---|---|
| `index.html` | Website markup, styles, catalogue data and client-side interactions |
| `assets/vayanvesha-mark.svg` | Compact brand mark |
| `assets/vayanvesha-logo.svg` | Horizontal wordmark |
| `assets/vayanvesha-app-icon.svg` | Scalable app icon |
| `assets/vayanvesha-social-preview.svg` | Editable social-sharing artwork |
| `favicon.svg` | Browser tab icon |
| `site.webmanifest` | Web app name, theme and install metadata |
| `SOURCES.md` | Source register, verification notes and legacy-record caveats |
| `DESIGN.md` | Brand, interface and implementation design decisions |
| `LICENSE` | MIT license for this repository's code, subject to the terms in that file |

The repository is currently named `lunivo`, so its GitHub Pages project address still contains that earlier name. The product and website brand is **Vayanvesha**. The repository name and public URL can be migrated after a custom domain is selected.

## Run locally

No build tools are required.

1. Clone or download this repository.
2. Open `index.html` in a modern browser.

For a local HTTP preview, run a static file server from the repository root, for example:

```bash
python -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000).

## Contributing and corrections

Resource suggestions and broken-link reports are welcome.

- [Suggest a resource](https://github.com/kr-ndv/lunivo/issues/new?title=Suggest%20a%20resource)
- [Report a broken destination](https://github.com/kr-ndv/lunivo/issues/new?title=Report%20a%20broken%20link)
- [Browse open issues](https://github.com/kr-ndv/lunivo/issues)

When suggesting a listing, please include the provider's official URL, a short explanation of its educational or research value, the intended audience if known, and a supporting official source. Please flag access restrictions, regional limitations or uncertain ownership rather than guessing.

Suggestions are reviewed manually. An issue submission does not guarantee inclusion, and there is currently no automated submission or moderation system.

## Brand

The name **Vayanvesha** is a coined brand blend inspired by Malayalam *vayana* (reading) and Sanskrit *anvesha* (inquiry or exploration). It is not presented as a traditional dictionary word.

The visual identity uses an Open Book + Discovery mark and this palette:

| Colour | Hex | Role |
|---|---|---|
| Deep olive | `#283618` | Primary dark background |
| Olive | `#606c38` | Book page and secondary surfaces |
| Warm cream | `#fefae0` | Light background and contrast |
| Amber | `#dda15e` | Discovery detail and highlight |
| Terracotta | `#bc6c25` | Secondary accent |

**Tagline:** Discover beyond boundaries.

## License

The repository includes an [MIT License](LICENSE) for its code. This does not automatically relicense third-party websites, catalogue content, provider logos, books, articles, datasets or other linked material. Those remain subject to their respective owners' terms, copyright and licenses. Check the rights attached to each resource before copying, redistributing or adapting it.

---

<div align="center">
  <sub>Vayanvesha · Read. Seek. Discover.</sub>
</div>

# CalmMind Therapy website

A static HTML/CSS/JavaScript website for CalmMind Therapy. The existing page title names Dr. Aanya Mehra. The original branding, page description, practice content and enquiry form are preserved.

## Local preview

Serve this directory with a static web server, for example `python -m http.server 8000`, then open `http://localhost:8000`.

External fonts, styles, scripts and images require an internet connection. There is no package manifest, configured lint suite or build command.

## SEO metadata

`index.html` includes developer author/creator metadata, Open Graph metadata, Twitter card metadata and one WebSite JSON-LD block identifying TheBenzzCreations as the website creator. This describes website development; it does not verify clinical authorship, professional credentials, treatment claims or testimonials. No medical business or review schema has been added.

The existing footer includes one visible developer credit with a normal same-tab hyperlink for the developer link.

Production identity is recorded in `seo-sites.json`; see Canonical URL validation below. The developer credit is not evidence of a project deployment URL.

## Development & Maintenance

**Developed & Maintained by
[Khushal Sehrawat](https://github.com/khushalsehrawat)**
— Founder of
[TheBenzzCreations](https://www.thebenzzcreations.com/).

TheBenzzCreations is a digital development studio specializing in website development, custom software, mobile applications, e-commerce solutions and AI-powered business automation.

For development enquiries and collaborations, visit [TheBenzzCreations](https://www.thebenzzcreations.com/).

## Canonical URL validation

Run `python scripts/validate_seo.py` from this repository before publishing. The dependency-free check validates exact page canonicals, Open Graph URLs, website/application JSON-LD URLs, sitemap locations, robots sitemap references and literal framework site metadata against `seo-sites.json`. It checks deployment path prefixes as well as domains, so one GitHub Pages project cannot canonicalize to another.

Only URLs whose live HTML matched the local page on 2026-11-21 are configured. Unverified pages have no canonical or social URL; `python scripts/validate_seo.py --require-verified` also fails for those pending pages. Reverify the configuration if the deployment moves. Dynamic framework expressions still require runtime validation.

TheBenzzCreations attribution, creator organization URLs and existing normal same-tab developer credit links are preserved. These outbound attribution links are separate from site identity.

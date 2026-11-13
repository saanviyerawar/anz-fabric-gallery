# ANZ Fabric Gallery

An Australia and New Zealand Microsoft Fabric app gallery, inspired by
[Fabric Apps](https://kornalexander.github.io/Fabric-Apps/).
The source lives in [saanviyerawar/anz-fabric-gallery](https://github.com/saanviyerawar/anz-fabric-gallery).
It is a standalone HTML/CSS/JavaScript site with no build step, package install,
external scripts, API keys, or Fabric tenant connection.

Open `index.html` in a modern browser, or serve this directory with an existing
static web server. The same file can be published with GitHub Pages from the
repository root. No deployment has been configured.

### Gallery content

- The page follows the original gallery layout: a text-led hero with inline
  statistics, category headings and preview-card grids, a project setup section,
  and three explanatory cards.
- All eight entries are placeholders named "Project 01" through "Project 08".
  They retain the four category groups (3 geospatial, 1 analytical, 2 platform
  tools, 2 games/learning) without claiming real project names or availability.
- Each card shows "Preview coming soon" and a "Coming soon" badge. Cards are
  non-interactive; there are no project links, media downloads, creator credits
  or confirmed locations. Setup instructions are also placeholders.
- Expand "Filter projects" to search by placeholder name or category.
  All project regions are currently marked `tbc` (to be confirmed).
- "Propose an app" opens a prefilled GitHub issue in this repository; it requires
  GitHub sign-in and maintainer review. It does not automatically publish a
  submission.
- Edit the `apps` array in `index.html` to rename or organise the placeholders.
  Each entry has a `title`, category (`geo`, `analytics`, `tools`, `learning`)
  and region (`tbc`). Update the card renderer, region filter and publication
  statistics when introducing confirmed project details, media or links.
- Category and placeholder counts derive from the catalogue. The page explicitly
  states that zero projects have been published.
- The theme follows the device preference unless `?clawpilotTheme=light` or
  `?clawpilotTheme=dark` is supplied. The theme button updates this URL parameter.
  Colours use Australian-flag-inspired navy and white, with a blue-grey dark
  theme. Shared CSS colour tokens keep buttons, links, badges and focus states
  consistent.

The layout is adapted from Alexander Korn's MIT-licensed
[Fabric Apps collection](https://github.com/KornAlexander/Fabric-Apps).
No projects or media from that collection are currently shown in the gallery.
See [THIRD_PARTY_NOTICES.txt](THIRD_PARTY_NOTICES.txt) for the upstream licence.
This is an independent community gallery, not an official Microsoft or ANZ Bank
site.

# ANZ Fabric Gallery

An Australia and New Zealand Microsoft Fabric app gallery, inspired by
[Fabric Apps](https://kornalexander.github.io/Fabric-Apps/).
The source lives in [saanviyerawar/anz-fabric-gallery](https://github.com/saanviyerawar/anz-fabric-gallery).
It is a standalone HTML/CSS/JavaScript site with no build step, package install,
external scripts, API keys, or Fabric tenant connection.

Open `index.html` in a modern browser, or serve this directory with an existing
static web server. The live gallery is published at
[saanviyerawar.github.io/anz-fabric-gallery](https://saanviyerawar.github.io/anz-fabric-gallery/).
GitHub Pages publishes from the repository root on `main`; pushed changes are
deployed automatically.

### Gallery content

- The page follows the original gallery layout: a text-led hero with inline
  statistics, category headings and preview-card grids, a project setup section,
  and three explanatory cards.
- The first entry is [Translink Community Impact Studio](https://github.com/AfsanehGhasemiGh/translink),
  contributed by AfsanehGhasemiGh: a Brisbane transport map, Fabric ontology
  chat and illustrative what-if demo. It is an independent concept demo, not
  an official Translink service or live journey planner.
- Seven entries remain placeholders named "Project 02" through "Project 08".
  The four category groups retain 3 geospatial, 1 analytical, 2 platform
  tools and 2 games/learning spaces.
- Each card has a category-specific inline SVG icon (globe, chart, tools or
  games). Placeholder cards have a numbered title and a single "Placeholder"
  badge. The icons are decorative, not project previews. The Translink card shows access
  requirements, a summary, contributor credit, and Request access, Open app and
  Source links. Remaining placeholder cards are non-interactive.
- Expand "Filter projects" to search by placeholder name or category.
  Category filters, search and reset controls are available; region filtering
  is omitted while locations remain unconfirmed.
- "Propose an app" opens a prefilled GitHub issue in this repository; it requires
  GitHub sign-in and maintainer review. It does not automatically publish a
  submission.
- Edit the `apps` array in `index.html` to rename or organise the placeholders.
  Each entry has a `title` and category (`geo`, `analytics`, `tools`, `learning`).
  Listed apps also have `description`, `creator`, `source` and `demo` fields.
  Search includes descriptions, contributors and access status.
- Project-space, listed-app and category counts derive from the catalogue.
  There is currently one listed app and seven placeholders.
- The theme defaults to light regardless of the device preference. Use
  `?clawpilotTheme=light` or `?clawpilotTheme=dark` to override it; missing or
  invalid values default to light. The theme button updates this URL parameter.
  Colours use Australian-flag-inspired navy and white, with a blue-grey dark
  theme. Shared CSS colour tokens keep buttons, links, badges and focus states
  consistent.

### Translink access requests

The [Request access form](https://github.com/saanviyerawar/anz-fabric-gallery/issues/new?template=translink-access.yml)
opens a public GitHub issue in this repository using
`.github/ISSUE_TEMPLATE/translink-access.yml`. It requires GitHub sign-in and
explicit acknowledgement of the manual approval process. Do not collect email
addresses, tenant identifiers, credentials or other personal information in
issues.

Maintainer and tenant-administrator process:

1. Review the request and arrange an approved private channel for the requester's
   sign-in details. GitHub issues have no private messaging; no private contact
   destination is configured by this site.
2. Verify the account and complete tenant onboarding or guest invitation if
   required by the tenant's policies.
3. Add approved users to the existing **Translink Demo Users** Entra security
   group. The app repository documents Viewer workspace access for this group;
   verify effective app **Read and execute** permission rather than assuming
   membership alone is sufficient. Do not grant workspace editing, administrator
   roles or ownership.
4. Ask the user to sign in to the [Fabric-hosted app](https://wide-grove-1455796ee4-westus.webapp.fabricapps.net/)
   with the approved account. Registration, MFA, licensing and tenant policy
   requirements remain enforced.
5. Confirm that the user can interact with the app before closing the request.
   Post only a non-sensitive completion status publicly; keep account details
   and access troubleshooting in the private channel.

This repository only records requests. It has no tenant credentials, Microsoft
Graph integration, automatic group membership or permission-granting backend.
The access process is documented, not proof that any new user has been approved
or successfully onboarded.

The layout is adapted from Alexander Korn's MIT-licensed
[Fabric Apps collection](https://github.com/KornAlexander/Fabric-Apps).
No projects or media from that collection are currently shown in the gallery.
See [THIRD_PARTY_NOTICES.txt](THIRD_PARTY_NOTICES.txt) for the upstream licence.
This is an independent community gallery, not an official Microsoft or ANZ Bank
site.

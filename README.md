# GENEXXO — Taxonomy Sandbox

A shareable, self-contained fork of the GENEXXO mobile network home page, used to
build out the **sector + gateway lists** at scale before they go back into the live shell.

## View it

- **Live:** once GitHub Pages is enabled → `https://<user>.github.io/<repo>/`
- **Locally:** open `network-home-sandbox.html` in any modern browser.

All video/imagery loads from the public `genexxo-vision.github.io` origin, so the page
renders fully from anywhere — no media files or the ecosystem repo are needed here.

## What's inside

| File | Purpose |
| :-- | :-- |
| `network-home-sandbox.html` | The sandbox app (the network home page + Sectors/Gateways drawers + Discover). |
| `Adventure.md` | Source list for the **Adventure** sector's gateways (grouped by sub-category). |
| `Sports.md` | Source list for the **Sports** sector's gateways (grouped by sub-category). |
| `index.html` | Redirect to the sandbox so the root URL just works. |

## How the lists work

Inside the sandbox's script, two structures drive everything:

- `const SECTORS = [ … ]` — the sector tiles.
- `const SECTOR_GATEWAYS = { … }` — each sector's gateway list. A `'#Group Name'`
  entry is a **sub-group header** (rendered as a divider), everything else is a gateway.

Open the right **Gateways** drawer on Adventure or Sports (or **Discover** → filter to that
sector) to see the grouped lists with their sub-headers.

> Sandbox only — this file is never deployed to the production ecosystem site.

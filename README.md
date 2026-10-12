# OceanSideVR hub site

Static company hub for oceanside-vr.com. Upload the contents of this folder
(not the folder itself) to the root of a repo named exactly `jmez11.github.io`.

## Setup

1. **Move the custom domain off the DeadEasy Player repo.** A domain can only
   live on one Pages site. In `jmez11/deadeasy-player`: Settings → Pages →
   Custom domain → delete `oceanside-vr.com` → Save.
2. **Create the hub repo** `jmez11.github.io` (public).
3. **Upload these files** to the repo root (unzip first; drag-and-drop in the
   GitHub web UI works). The `CNAME` file tells Pages the domain automatically.
4. **Enable Pages:** repo Settings → Pages → Source: *Deploy from a branch* →
   branch `main`, folder `/ (root)` → Save.
5. **HTTPS:** once GitHub verifies DNS (usually minutes), tick *Enforce HTTPS*
   under Settings → Pages.

DNS stays exactly as it is — the four `A` records and the `www` CNAME already
point at GitHub Pages.

## What happens to DeadEasy Player

Nothing breaks. Its project site automatically becomes
`oceanside-vr.com/deadeasy-player/` — a path under the hub, no subdomain.
Old links like `jmez11.github.io/deadeasy-player/PRIVACY.html` (including the
one on the Meta store listing) redirect to the new address.

## Files

- `index.html` — the hub page
- `styles.css` — dark theme with neon accent
- `assets/logo.png` — brand icon (from the DeadEasy Player site)
- `CNAME` — `oceanside-vr.com`, picked up by Pages automatically

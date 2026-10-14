# Mr. Defendable — landing base

Sovereign CRE intelligence. **The intelligence comes to the lease. The lease never leaves.**

Static landing page for `mrdefendable.com`, built for Cloudflare Pages. This is the **base** — hack/agent modules insert at the mount points.

## Deploy (Cloudflare Pages)
- Framework preset: **None** (static).
- Build command: *(none)*
- Build output directory: **`/`** (repo root; `index.html` is served directly).
- Custom domain: `mrdefendable.com`.

No build step, no dependencies — just `index.html`. Fonts load from Google Fonts; everything else is inline.

## Structure
- `index.html` — the whole page (brand palette "Honey & Ink" locked in the `:root` tokens).
- Sections, in order: hero → the wall (pain) → why defendable (two locks) → the machine (edge + fleet) → the voice → the lane (1031 clock) → the deal (deliver/don't) → **hacks mount** → close.

## Inserting hacks
The fleet section (`#hacks`) carries the mount point:

```html
<div class="slot" data-slot="hacks"> … </div>
```

Replace that node with per-vertical specialist cards (industrial, net-lease, retail, multifamily). Reuse the existing `.tcard` / `.lock` / `.col` components and the `:root` tokens so inserts stay on-brand. One hack per vertical; each starts `hackN.onshine.mrdefendable.eth`.

## Brand tokens (Honey & Ink)
Accent honey `#a8741a` / `#c88a1b` bright · ink `#191c1a` · stone `#f1f0ec` · vault `#0e1013` · bankable green `#2f6b4c` · crickets rust `#a1361f`. Display **Libre Franklin**, serif voice **Newsreader**, data **IBM Plex Mono**. Light + dark + system all themed at the token level.

---
Verified · Vetted · Defendable · `mrd.defendable.eth`

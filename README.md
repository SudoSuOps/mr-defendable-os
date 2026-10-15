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
- Sections, in order: hero → the wall (pain) → why defendable (two locks) → the machine (edge + fleet) → **the ask (live STNL demo)** → the voice → **the climb (hack → contractor → builder)** → the lane (1031 clock) → **the gate (the moat)** → the deal (deliver/don't) → **the skills (5 hacks)** → close.

## The Ask demo (`#ask`)
Client-side STNL demo — the product surface: broker types a plain-English ask → Mr. Defendable returns one intelligence graph per box (credit, lease, owner→entity→person [person gated], debt, exchange→cap, seller signal, comp lineage). No backend; runs on Pages as-is. **Data in `DB` is illustrative, not live records** (fictional entities, person gated on purpose) — swap in a real gated API call where `run()` renders. Add tenants by extending the `DB` object and the `parse()` matchers.

## Inserting hacks
The fleet section (`#hacks`) now holds the five skills as `.skill` cards inside `<div class="skills" data-slot="hacks">`:

1. **Book Maker** (`hack1`) — the four-pager
2. **Legal Digest** (`hack2`) — lease red-flags
3. **Underwriter** (`hack3`) — P-close + debt-yield
4. **Social Heat Map** (`hack4`) — demand heat by market
5. **The Sourcer** (`hack5`) — the P-close list (MAKER→TAKER)

Add a skill by copying a `.skill` card and bumping the index + `hackN` handle. Each is a specialist model gated to its own `.eth`; the grid is 3-col → 2-col → 1-col responsive.

## Brand tokens (Honey & Ink)
Accent honey `#a8741a` / `#c88a1b` bright · ink `#191c1a` · stone `#f1f0ec` · vault `#0e1013` · bankable green `#2f6b4c` · crickets rust `#a1361f`. Display **Libre Franklin**, serif voice **Newsreader**, data **IBM Plex Mono**. Light + dark + system all themed at the token level.

---
Verified · Vetted · Defendable · `mrd.defendable.eth`

# Performance in every layer

Static, faithful recreation of the HOLCIM SYSTEMS "every layer" hero layout.

Open `index.html` in any browser — no build step, no dependencies.

## How the navigation works

The panels on the right are a **layer navigator**. Click any fanned sliver and it
animates to the front as the large panel, while the left content pane (heading,
body copy and the stat block) updates to describe that layer. Click-to-select only.

## Placeholder assets to replace later

Everything below is dummy content, ready to swap for the real brand assets:

| What | Where |
|------|-------|
| Layer photos | `assets/layer-1.svg` … `layer-5.svg` (referenced in the `LAYERS` array in `index.html`) |
| Content-pane thumbnail | `assets/stat-thumb.svg` |
| HOLCIM SYSTEMS logo | `assets/logo.svg` |
| Colours | `:root` CSS variables at the top of `index.html` (`--bg`, `--accent`, …) — all estimated from the reference, replace with exact hex |
| Fonts | `--font-display` (the light geometric "every layer" face) and `--font-body` in the same `:root` block |
| Copy / stats per layer | the `LAYERS` array in the `<script>` block |

Replace an `img` path or drop a same-named file in `assets/` and it appears with no
other changes.

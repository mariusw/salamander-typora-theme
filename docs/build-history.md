# Salamander Typora Theme — Build History

A living document. Add entries chronologically as milestones ship.

---

## v1 — Foundation: palette, typography, and bundled fonts (May 2026)

**What it was:** A single-day build that took the theme from nothing to a fully installable
Typora theme. The core design problem was establishing a warm dark palette that felt cohesive
rather than just dark-with-orange — a near-black background (`#0E0A06`) anchored in deep brown,
warm beige body text, and burnt orange as the primary accent. The aesthetic target was earthy
and readable, not stark or high-contrast.

**Key decisions:** Three font families were bundled as local woff2 files from the start — Syne
for headings, Plus Jakarta Sans for body, JetBrains Mono for code — rather than relying on system
fonts or web font fetches. This was a deliberate tradeoff: larger repo size in exchange for
offline-reliable rendering and full control over the typographic hierarchy. Full syntax
highlighting for code blocks was included in the initial scope rather than deferred.

**What shipped:** The complete `salamander.css` (378 lines in initial commit, expanded to ~450
after fixes), 12 bundled woff2 font files across three families, styled tables, math blocks
(KaTeX), task lists, and Mermaid diagrams. A `.gitignore`, initial README, and a `salamander.zip`
for distribution.

**Limitations that drove the next phase:** The initial state had no visual documentation — no
screenshots, no preview file — which made it difficult to assess the theme without installing it
and hard to present to others. The README was minimal.

---

## v2 — Documentation and visual preview (May 2026)

**What it was:** A focused documentation pass the same evening as the initial build. The goal
was to make the theme presentable: a preview Markdown file that exercises all the major style
rules, four screenshots capturing it in use, and a README that communicates the palette and
font choices clearly enough that someone could decide whether to install it before doing so.

**Key decisions:** Screenshots were added as static PNGs in a `preview/` folder and linked
directly from the README. A `preview.md` file was created as a controlled showcase document —
deliberately covering headings at every level, code blocks, tables, lists, and other styled
elements so that screenshots would be representative rather than cherry-picked.

**What shipped:** Four preview screenshots (`preview/1.png` through `preview/4.png`), the
`preview.md` showcase file, an expanded README with the full palette table and font table,
installation instructions, and a symlink-based development workflow.

**Limitations that drove the next phase:** The theme is ready to install and use, but has not
been submitted to the Typora community theme gallery. There is no release workflow, no versioning
beyond the initial zip, and no automated way to package a distribution archive.

---

## Open / Upcoming

- Submit to the official Typora theme gallery
- Set up a GitHub release workflow that builds and attaches the zip automatically
- Consider a light variant or a higher-contrast mode for readability in bright environments
- Add a `docs/design-decisions.md` capturing why specific palette values were chosen

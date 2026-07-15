# Final Polish — QA Checklist

Design director review before shipping.

---

## Spacing

- [x] Blank line before every `####` section header
- [x] Blank line after every section header
- [x] Blank line between every project card table
- [x] `assets/divider.svg` between major sections (hero → 01 → 02 → 03 → footer)
- [x] Hero → Section 01 gap feels like a page break (divider + blank line)
- [x] No tight stacking of headings on content

## Alignment

- [x] All content left-aligned except hero/footer SVG (centered via `<p align="center">`)
- [x] Analytics table cells center their images
- [x] Contribution graph centered
- [x] Label columns in tables at consistent width (~90px)
- [x] All left edges align to single invisible column

## Hierarchy

- [x] Hero: System title → Name → Domains → Metrics → Links
- [x] Sections numbered: 01, 02, 03
- [x] Winners before non-winners in hackathon list
- [x] Shipped Systems subsection below hackathon winners
- [x] Capability headings (`#####`) below section headings (`####`)
- [x] No skipped heading levels

## Consistency

- [x] Every hackathon card uses identical 4-row table schema
- [x] Every shipped product card uses identical 5-row table schema
- [x] All mono labels use backtick formatting
- [x] Link style: text descriptors (`repo` · `live` · `demo`), not icon-only
- [x] Accent color `#3b6fa8` used only in SVG assets and stats URL params
- [x] No emoji anywhere in profile
- [x] No banned tropes present

## Accessibility

- [x] All SVGs have `role="img"` and `aria-label`
- [x] All images have `alt` text
- [x] Links are text-described
- [x] Sufficient contrast in SVG (primary `#1a1a1a` on `#fafafa`)
- [x] Readable without color alone (labels + values paired)

## GitHub Compatibility

- [x] No JavaScript
- [x] No external CSS files
- [x] No iframes
- [x] SVGs contain no scripts or foreignObject
- [x] HTML tables used (GitHub renders them)
- [x] All asset paths relative (`assets/...`)
- [x] Stats/streak images use HTTPS URLs
- [x] Snake workflow configured for contribution graph
- [x] Tested SVG size < 5KB each

## Dark Mode

- [x] Markdown text uses GitHub defaults (auto-adapts)
- [x] SVG surfaces are light (`#fafafa`) — acceptable: hero/footer are intentional "document pages"
- [x] Stats cards use `bg_color=ffffff` — may appear bright in dark mode; acceptable trade-off for brand consistency
- [ ] **Monitor:** User feedback on dark mode SVG contrast

## Content Integrity

- [x] All 21 Devpost projects included
- [x] 9 international hackathon wins reflected in hero metrics
- [x] 10 shipped systems from aitch-cmd repos
- [x] No invented projects
- [x] No removed achievements
- [x] Username `aitch-cmd` consistent throughout

---

## Design Director Final Verdict

**Ship-ready** with one monitoring item (dark mode SVG contrast).

The profile reads as a single engineering specification document. Typography and spacing do the heavy lifting. No widget walls. No trope patterns. Hero and footer bookend the experience.

**Quality bar:** Premium engineering document ✓

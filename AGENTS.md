# Tiger Studio Public Page Agent Rules

These rules are for AI coding agents working on the public Tiger Studio /
TigerCapture distribution repository or GitHub Pages worktree.

## Required Start Point

Before editing the public website, README, product catalog, release page text,
or GitHub Pages layout, read:

1. `docs/PUBLIC_PAGE_SHOWCASE_STRUCTURE.md`
2. `docs/product_catalog/SPEC.md`
3. `README.md`

Use the showcase structure document as the page-direction source of truth.

## Public Repository Boundary

This public repository/worktree is for distribution-safe materials only:

- landing pages
- public docs
- catalog images
- screenshots
- release notes
- installers or packaged artifacts

Do not add implementation trees, tests, private build notes, unpublished branch
details, local diagnostics, or non-release materials.

## Brand Rules

- Main product name: `Tiger Studio`
- Do not use `TigerCapture` as visible product copy.
- `tigercapture` may remain only in repository URLs, package identifiers, or other technical continuity strings.
- Positioning: `Subculture-ready video editor for screen, shorts, and character creators.`
- Keep the page video-editor-first and character/subculture-ready.
- Do not let the page read as only a capture utility.

## Page Style Rules

- Use the visual showcase direction from
  `docs/PUBLIC_PAGE_SHOWCASE_STRUCTURE.md`.
- First viewport must clearly show `Tiger Studio`, the short product category,
  and a download CTA.
- Product Walkthrough should use a large left preview, a compact right-side
  scene index, and scroll-synced background imagery.
- Keep English as the main copy and Korean as supporting copy.
- Keep public claims honest and consistent with the public spec.

## Validation Checklist

Before committing public page changes:

- Verify referenced images and docs exist.
- Check that no non-release materials were added.
- Check that `TigerCapture` is not used as visible product copy.
- Keep `gh-pages` and `release` public page files in sync when both worktrees
  are being maintained.

# Dog Sitting — Front-End Dev Test

A responsive implementation of a banner and a card grid for a dog-sitting website.
Plain HTML and CSS, no frameworks.

## Approach & decisions

- **Design tokens** — colours, the type scale and layout values live as CSS
  custom properties in `:root`, taken from the Figma spec.
- **Breakpoints** — `768px` (tablet) and `1100px` (desktop).
- **Service cards**:
  - Mobile: single column, image on top
  - Tablet (≥768px): single column, image beside the text
  - Desktop (≥1100px): three columns, image on top
- **Hero** — background banner with layered gradient overlays, a white SVG wave,
  and a mobile-specific crop that keeps the dog centred.
- **Accessibility** — logical heading order, descriptive `alt` text, decorative
  elements hidden from assistive tech, and `:focus-visible` outlines for
  keyboard users.

## Design issues

- **Typos**:
  - "piece of mind" -> "peace of mind"
  - "someones else" -> "someone else's"
  - "Look no futher" -> "Look no further"
- **Colour contrast** — The orange `#FF6D00` fails WCAG AA for white on orange.
  Meeting AA would need a darker orange.

## AI use

Built with the help of Claude Code, used for the HTML/CSS, debugging responsive
layout, and drafting this README. All changes were reviewed and tested before commit.

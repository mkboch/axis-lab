# AXIS Lab resource portal — design system

## Context

- Artifact: static academic resource index.
- Primary audience: WANG-AXIS lab members looking for datasets, compute, roles, or code.
- Secondary audience: collaborators and visitors learning what the lab does.
- Primary outcome: reach the correct maintained resource or current member profile with minimal scanning.
- Positioning: academic and technical, not a software product or marketing campaign.

## Direction

- Brand adjectives: precise, credible, restrained, technical, human.
- Aesthetic essence: clinical editorial index.
- Signature move: a numbered, full-width resource directory paired with a live, restyled upstream roster.
- Restraint: no gradients, glass effects, soft shadows, decorative icon tiles, card grids, or autonomous animation.

## Tokens

- Display type: IBM Plex Serif, weight 500.
- Body/interface type: IBM Plex Sans, weights 400/500/600.
- Type scale: 1.25 ratio from a 16px base; 13, 16, 20, 25, 31, 49, 76px.
- Spacing: 4px base; relationship-driven groups use 8/12/20px and sections use 64/96/128px.
- Radius: 0 for structural elements; 2px for keyboard controls only.
- Elevation: no shadows. Hierarchy comes from type, spacing, rules, and surface contrast.

### Color roles

| Role | Value |
| --- | --- |
| Background | `oklch(0.985 0.003 240)` |
| Surface | `oklch(1 0 0)` |
| Foreground | `oklch(0.20 0.018 245)` |
| Muted | `oklch(0.49 0.025 245)` |
| Border | `oklch(0.84 0.012 240)` |
| Accent | `oklch(0.45 0.12 244)` |
| Accent surface | `oklch(0.94 0.025 236)` |
| Focus | `oklch(0.66 0.16 70)` |

## Layout and interaction

- Desktop composition uses a 12-column grid with deliberate asymmetry.
- Resource links are rows, not cards; their shared alignment makes them scannable.
- Links stay visibly underlined or gain an explicit background on hover.
- The only scripted interaction is the mobile navigation toggle.
- Focus is visible, targets are at least 44px tall, and reduced-motion preferences are respected.
- Mobile collapses to one reading column without changing the information order.
- The People page fetches and sanitizes the official upstream members page at runtime, then presents it with the local design system.
- Member photographs retain their upstream color and complete original aspect ratio; the local layout never crops them.

## Slop audit

- No centered gradient hero.
- No Inter/system font as the primary face.
- No icon-in-rounded-square cards.
- No decorative eyebrow above every section.
- No fake metrics, testimonial strip, oversized CTA panel, or arrow appended to every link.
- No repeated equal-weight section templates.
- Numbering is used only for the resource directory, where sequence and cross-reference are meaningful.
- Color supports hierarchy but does not create it.

## Changelog

- 2026-11-24: Replaced the generic SaaS-style portal with the clinical editorial index direction.
- 2026-11-24: Added a synchronized People tab and removed decorative imagery from the landing page.

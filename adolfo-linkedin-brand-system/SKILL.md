---
name: adolfo-linkedin-brand-system
description: Create visually consistent, high-impact LinkedIn assets for Adolfo Salas, GoalPraxis, and mining/asset-performance advisory content. Use this skill whenever the user asks for Adolfo's LinkedIn brand, visual identity, post design, carousel design, PDF carousel, single-image ad, lead magnet, personal brand visuals, GoalPraxis visual style, mining executive content design, or wants to combine LinkedIn service-offer copy with canvas, Slidev, PPTX, Gemini image generation, Firecrawl, or Playwright research.
---

# Adolfo LinkedIn Brand System

Use this skill to turn Adolfo's mining operations expertise and advisory offers into a consistent visual language for LinkedIn.

This skill is visual and production-oriented. Pair it with `linkedin-service-offer-ads` when the user needs both copy/offer strategy and publishable visual assets.

## Brand Position

Adolfo is not positioned as a generic influencer or software vendor. Position him as:

- Mining operations and technology leader
- Operator-builder-advisor
- Asset performance and maintenance transformation specialist
- AI/BI and predictive maintenance translator for real operations
- Executive-level, grounded, analytical, practical
- Latin America mining experience with global advisory perspective

Default brand sentence:

```text
Mining operations intelligence for leaders who need asset data to become decisions, execution, and measurable business results.
```

## Visual Personality

The visual identity should feel:

- Executive, not decorative
- Analytical, not academic
- Industrial, not heavy-handed
- Technology-forward, not futuristic cliché
- Premium, not flashy
- Human and practical, not software-vendor generic

The work should look like it belongs between a mining executive briefing, a serious consulting diagnostic, and a design-forward technology report.

## Core Palette

Use this palette by default:

| Name | Hex | Use |
|---|---:|---|
| Graphite | `#101820` | Dark backgrounds, executive authority |
| Mineral White | `#F6F1E8` | Main light background |
| Copper | `#B86B3D` | Primary accent, mining/material signal |
| Deep Teal | `#0E746E` | Technology, systems, decision flow |
| Signal Blue | `#2F80ED` | Sparing data/AI accent |
| Stone Gray | `#66727A` | Secondary copy and labels |
| Sand Line | `#C9B8A4` | Dividers, grid lines, subtle structure |
| Alert Amber | `#E0A33A` | Rare warning/diagnostic accent |

Rules:

- Do not let teal or copper dominate every element.
- Use Graphite + Mineral White as the base contrast.
- Use Copper as the mining/material accent.
- Use Deep Teal for flow, systems, and technology logic.
- Use Signal Blue only when the subject is AI, data, or digital signal.
- Avoid purple-heavy gradients, soft startup SaaS palettes, beige-only palettes, and generic neon tech styling.

## Typography

Use clean, serious typography. Prefer system fonts for reliability:

- Headings: Arial Bold, Segoe UI Semibold, Aptos Display, or similar strong sans-serif
- Body: Arial, Segoe UI, Aptos, or similar neutral sans-serif
- Labels: small uppercase, letter spacing only if legible

Rules:

- Use large headlines with short line lengths.
- Use body text sparingly on images.
- Never use paragraphs inside carousel slides.
- Use sentence case more than title case.
- Avoid playful fonts, script fonts, and generic tech display fonts.

## Signature Motifs

Use these visual motifs repeatedly so the brand becomes recognizable:

- Signal-to-action flow: signal -> decide -> plan -> execute -> learn
- Decision cadence maps
- Asset performance system diagrams
- Mining fleet grids and operational cells
- Copper horizontal bars or thin line markers
- Technical labels and diagnostic numbering
- Layered maps: data, decision, execution, business impact
- Sparse top rule or side rule for executive-report feel
- Subtle mineral/terrain linework, never cartoon mining icons

Avoid:

- Stock-photo hero clichés
- Generic AI robot imagery
- Overused dashboard mockups without meaning
- Overcrowded infographic cards
- Decorative blobs, bokeh orbs, and random gradients
- Tiny unreadable labels on LinkedIn mobile

## LinkedIn Formats

### Text-Only Post

Use the brand voice but no visual design. Structure:

1. Short hook
2. 2-4 short paragraphs
3. Practical bullets or diagnostic questions
4. Clear CTA

### PDF Carousel / Document Post

Default specs:

- 1080x1350 portrait
- 6-8 pages
- One idea per page
- 18-35 words per page where possible
- Strong first slide hook
- Last slide CTA
- Export as PDF for LinkedIn document upload
- Also save PNG pages when useful

Slide structure:

1. Hook
2. Problem
3. Hidden cause
4. Framework/system
5. Diagnostic or proof point
6. Offer
7. CTA

### Single-Image Post / Ad

Default specs:

- 1200x1200 square for organic or broad compatibility
- 1200x627 landscape for sponsored content when requested
- One dominant headline
- One simple visual system or diagram
- One clear CTA or brand signature

### Lead Magnet / Checklist

Default specs:

- 4-6 pages
- 1080x1350 portrait
- Utility-first design
- Checklists, diagnostic questions, decision maps
- Caption CTA: comment or DM a keyword

### Poll Post

No graphic required. Use the visual system only if turning the poll into a follow-up carousel.

## Copy And Visual Integration

When paired with `linkedin-service-offer-ads`:

1. Let `linkedin-service-offer-ads` define the buyer, pain, offer, CTA, and slide copy.
2. Use this skill to select visual format, palette, hierarchy, motif, and export assets.
3. Keep slide text short even if the copy source is longer.
4. Preserve a grounded operator-advisor voice.
5. Make the final output publishable, not only strategic.

## Tool Selection

Use tools this way:

- `canvas-design`: for a highly visual single image, poster, or premium static ad.
- `slidev`: for editable, repeatable carousels and PDF export.
- `pptx`: for business-editable decks.
- Gemini image generation: for background imagery or abstract mining/technology visuals, not for final text rendering.
- Firecrawl MCP: for public research, examples, competitor pages, and source extraction.
- Playwright MCP: for JavaScript-heavy pages, visible design inspection, screenshots, and rendered examples.

When an image model is used, render final text yourself in code, Slidev, PPTX, or design tooling so LinkedIn text remains crisp and editable.

## Production Output Rules

When asked to create publishable assets, provide:

- Final asset files: PDF, PNG, JPG, or PPTX as appropriate
- Source/editable file when feasible
- Caption/copy file
- README explaining what to publish and where
- Optional individual carousel PNG pages

Use this folder naming pattern in the workspace:

```text
LinkedInAIPosts/[campaign-name]/
```

Recommended file names:

- `carousel.pdf`
- `single-image.png`
- `single-image.jpg`
- `lead-magnet.pdf`
- `caption.md`
- `README.md`

## Quality Checklist

Before finalizing a visual output, verify:

- It is legible on mobile.
- The first slide or image has a strong hook.
- The palette feels executive and mining-relevant.
- Text does not overlap or crowd the canvas.
- One idea dominates each visual.
- The CTA is visible but not desperate.
- The output feels like Adolfo: practical, analytical, serious, and useful.
- The asset is publishable without additional design work.

## Example Prompts This Skill Should Handle

- "Use my LinkedIn brand system to make this carousel look more premium."
- "Create a GoalPraxis single-image LinkedIn ad about dashboards and decisions."
- "Make a 7-slide PDF carousel using linkedin-service-offer-ads and my brand system."
- "Generate a lead magnet checklist in Adolfo's mining executive visual style."
- "Use Gemini for a background image, but render final LinkedIn text crisply."
- "Research visual inspiration with Playwright, then create an original LinkedIn post design."

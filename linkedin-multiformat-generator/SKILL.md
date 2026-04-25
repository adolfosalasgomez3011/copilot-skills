---
name: linkedin-multiformat-generator
description: Generate premium LinkedIn content systems across all major formats (text post, single image, carousel PDF, lead magnet, infographic, GIF, and MP4 video). Use this skill whenever the user asks for LinkedIn post generation, LinkedIn content templates, campaign systems, reusable pipelines, post variants, visual posts, infographic posts, animated posts, video posts, or wants a single workflow that can repeatedly produce high-quality LinkedIn assets.
---

# LinkedIn Multiformat Generator

Use this skill to create repeatable, publishable LinkedIn campaigns from one strategic idea across all common post formats.

This skill orchestrates strategy, copy, design, and exports. It is intended to be reusable as a template system, not a one-off output.

## Positioning

Treat this as an executive-grade content engine:

- One core message
- Multiple publishing formats
- Consistent visual identity
- Format-specific optimization
- Reproducible outputs

When possible, pair with:

- `linkedin-service-offer-ads` for offer and copy strategy
- `adolfo-linkedin-brand-system` for visual language and quality bar
- Gemini image generation for text-free visual backgrounds only

## Trigger Conditions

Use this skill whenever the user asks for:

- "all LinkedIn post types"
- "template for LinkedIn generator"
- "content system" or "content engine"
- "one idea in multiple formats"
- "animated LinkedIn post"
- "infographic + video"
- "carousel + single image + video"
- "reusable workflow for LinkedIn"

Use it even if the user only says "make a LinkedIn post generator" because the likely intent is multi-format production.

## Input Brief Template

Before generating assets, gather or infer:

- Audience: who should care
- Core problem: what is broken today
- Core promise: what changes
- Proof anchors: numbers, experience, evidence
- CTA keyword: one low-friction action
- Tone: advisory, contrarian, educational, direct response
- Primary visual metaphor: one clear concept

If details are missing, proceed with reasonable defaults and label assumptions.

## Format Output Matrix

For each campaign, produce:

1. Text-only post
2. Single image post (PNG/JPG)
3. Carousel document (PDF + optional pages)
4. Lead magnet document (PDF)
5. Infographic static post (PNG)
6. Infographic animated GIF
7. Short MP4 video version (if dependency available)
8. Captions file with variants
9. README with publishing order
10. Source generator scripts when feasible

## Visual and Motion Rules

- Use Gemini for background texture only.
- Do not rely on model-rendered text.
- Render final text, labels, CTA, and chart annotations in code/design tools.
- Keep mobile readability first.
- For motion, animate one core mechanism (progression, chart growth, stage highlight) instead of many effects.
- Keep loop duration short and clear (8-20 seconds for LinkedIn feed-friendly clips).

## Recommended Dimensions

- Single image: 1200x1200
- Carousel / lead magnet pages: 1080x1350
- Infographic static: 1080x1080
- GIF/MP4 motion: 1080x1080 (or 1080x1350 when requested)

## Text-Safe Gemini Protocol

When prompting an image model:

- Explicitly request no text, no letters, no numbers, no logos, no UI
- Request clean negative space for overlays
- Generate 2-4 variants
- Reject backgrounds containing fake UI labels or accidental words
- Darken/blur background if needed before overlay

## Generation Workflow

1. Build the campaign narrative: hook, mechanism, proof, action.
2. Generate text-safe background variants.
3. Select one winning background per format set.
4. Render static assets with code-based typography.
5. Render motion assets (GIF first, MP4 optional fallback).
6. Validate dimensions, readability, and output file presence.
7. Deliver publish-ready package plus source files.

## Quality Gate

Before finalizing:

- Hook is visible in first 2 seconds (for motion) or first glance (static)
- At least one graph or data motif exists where relevant
- Icons are legible on mobile
- CTA is singular and obvious
- Text contrast is strong
- No overlapping elements
- No hallucinated model text in final export

## Required Delivery Structure

Place outputs under:

`LinkedInAIPosts/<campaign-name>/`

Recommended file names:

- `caption.md`
- `README.md`
- `single-image.png`
- `single-image.jpg`
- `carousel.pdf`
- `lead-magnet.pdf`
- `infographic-static.png`
- `infographic-motion.gif`
- `infographic-motion.mp4`
- `generate_*.py`

## MCP Template Integration

This skill includes an MCP blueprint at:

- `references/mcp-blueprint.md`

Use that blueprint when the user asks to operationalize this workflow as callable MCP tools.

## Example Prompts This Skill Should Handle

- "Create one LinkedIn campaign in all formats including video"
- "Make an infographic post plus GIF and MP4"
- "Build me a reusable LinkedIn generator template"
- "Turn this service offer into carousel, image, and motion assets"
- "Package this as a system I can reuse every week"

# MCP Blueprint: LinkedIn Multiformat Generator

Use this blueprint to build a dedicated MCP server that exposes repeatable tools for LinkedIn asset production.

## Goal

Provide tool endpoints that convert one campaign brief into a full set of LinkedIn assets:

- strategy and copy
- static visuals
- document exports
- motion outputs

## Suggested Tool Set

1. `linkedin_generate_brief`
- Input: audience, pain, promise, CTA keyword, tone
- Output: normalized campaign brief

2. `linkedin_generate_copy_pack`
- Input: normalized brief
- Output: hook variants, caption variants, carousel slide copy, CTA variants

3. `linkedin_generate_textsafe_backgrounds`
- Input: visual metaphor, palette, count
- Output: paths to generated no-text backgrounds

4. `linkedin_generate_static_assets`
- Input: copy pack + background + format spec
- Output: single image, infographic static, optional carousel pages

5. `linkedin_generate_document_assets`
- Input: copy pack + style spec
- Output: carousel PDF and lead magnet PDF

6. `linkedin_generate_motion_assets`
- Input: infographic spec + timing/fps
- Output: GIF and MP4

7. `linkedin_validate_outputs`
- Input: folder path
- Output: dimension checks, missing file checks, quality flags

8. `linkedin_publish_package`
- Input: folder path
- Output: final README and publishing sequence

## Suggested Data Models

### CampaignBrief
- campaign_name
- audience
- core_problem
- core_promise
- proof_points[]
- cta_keyword
- tone
- visual_metaphor

### CopyPack
- hooks[]
- captions[]
- carousel_slides[]
- lead_magnet_sections[]
- cta_variants[]

### AssetSpec
- format_type
- width
- height
- palette
- background_path
- typography_profile
- animation_profile

## Implementation Notes

- Prefer TypeScript MCP SDK or FastMCP Python.
- Return structuredContent with output file paths.
- Use actionable errors (missing dependencies, missing background, invalid dimensions).
- Support idempotent re-runs with `campaign_name` and `overwrite` flags.

## Suggested Server Name

`linkedin-multiformat-mcp`

## Tool Naming Convention

Use consistent prefixing:

- `linkedin_generate_*`
- `linkedin_validate_*`
- `linkedin_publish_*`

## Minimal Rollout Plan

Phase 1:
- brief + copy + validate tools

Phase 2:
- static + document generation tools

Phase 3:
- motion generation and packaging tools

## Acceptance Criteria

A single toolchain run should produce:

- text post copy
- single image
- carousel PDF
- lead magnet PDF
- infographic static
- GIF
- MP4 (or clear dependency warning)
- caption and README

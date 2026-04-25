---
name: linkedin-service-offer-ads
description: Create LinkedIn service-offer ads, organic posts, document carousels, single-image ad briefs, and campaign variants for consultants, advisors, founders, and B2B service providers. Use this skill whenever the user asks for LinkedIn ads, LinkedIn carousels, service offers, lead generation posts, paid LinkedIn creative, personal-brand monetization, consulting offers, advisory offers, or content that promotes professional services, even if they say only "post", "ad", "carousel", "offer", "campaign", or "sell my services".
---

# LinkedIn Service Offer Ads

Use this skill to turn expertise into LinkedIn content that can generate trust, conversations, and leads without sounding desperate or generic.

The default user context is a senior mining operations and technology leader building a portfolio career around advisory, consulting, and company-building. His strongest service themes are:

- Mining asset performance transformation
- Maintenance and reliability improvement
- Predictive maintenance, IoT, dashboards, AI-enabled BI, and real-time monitoring
- Technology strategy that connects operational data to business results
- C-suite and COO-level advisory for mining operators
- Independent consulting and GoalPraxis offers
- Latin America mining experience, global advisory perspective, Spanish/English capability

If the task is for a different user or business, adapt the same framework to the new context.

## Core Positioning

Favor a high-trust advisor tone. The user is not a beginner selling a commodity service. Position him as an operator-builder-advisor with lived mining experience.

Default positioning statement:

```text
I help mining operators turn underperforming assets, fragmented data, and maintenance complexity into reliable performance, lower cost, and clearer executive decisions.
```

Default proof points to use only when relevant:

- 25+ years in mining operations, asset management, technology, and advisory
- 16 years client-side operations experience
- $500M+ mining portfolios
- 600+ technician service organizations
- 20-40% availability or performance improvement potential when supported by actual context
- 15-25% maintenance cost reduction potential when supported by actual context
- Operator, supplier, consultant, and entrepreneur perspective

Do not invent client names, numbers, certifications, revenue, or case studies. If proof is missing, use softer phrasing such as "in similar mining environments" or ask for details.

## Best Format Recommendation

When the user asks what to publish, recommend this order:

1. Document carousel/PDF post for the main service offer.
2. Single-image post/ad for direct-response testing.
3. Text-only authority post for trust-building.
4. Paid LinkedIn ad only after the organic angle shows traction.

Default carousel specs:

- 1080x1350 portrait pages
- 6 to 8 slides
- One idea per slide
- Large readable text
- Minimal copy, strong contrast
- Export as PDF for LinkedIn document post

Default paid ad specs:

- Single Image Sponsored Content: 1200x1200 or 1200x627
- Document Ad: short PDF guide or diagnostic framework
- Lead Gen Form: use only after the offer is specific and the CTA is tested organically

## Offer Angles

Generate 3 to 5 angles before writing final assets unless the user already chose one.

Use these angle families:

- Pain-to-outcome: "Your fleet data is visible, but decisions are still slow."
- Diagnostic: "5 signs your maintenance strategy is leaving money underground."
- Contrarian: "Most predictive maintenance projects fail before the algorithm matters."
- Executive lens: "What COOs need from asset performance dashboards."
- Operator truth: "The dashboard is not the transformation. The operating rhythm is."
- Lead magnet: "Comment 'audit' and I will send the mining asset performance checklist."
- Founder/advisor offer: "I help mining teams bridge the gap between technology investment and measurable performance."

## Required Output Structure

For a complete LinkedIn service-offer package, produce:

```markdown
# LinkedIn Service Offer Package

## Recommended Format
[State the best format and why]

## Audience
[Target buyer, decision-maker, and secondary audience]

## Offer
[One sentence offer]

## Core Message
[One sentence positioning]

## Creative Angles
[3-5 distinct campaign angles]

## Primary Carousel
Slide 1: [hook]
Slide 2: [problem]
Slide 3: [why it happens]
Slide 4: [framework]
Slide 5: [proof or example]
Slide 6: [offer]
Slide 7: [CTA]

## LinkedIn Caption
[Organic post copy, 900-1,300 characters unless user asks otherwise]

## Single-Image Ad Variant
Headline: [max 70 chars]
Text: [max 150 chars for ad preview]
Image concept: [visual brief]
CTA: [comment/DM/lead form]

## A/B Test Variants
Variant A: [pain-led]
Variant B: [outcome-led]
Variant C: [authority-led]

## Production Notes
[Design format, asset requirements, export notes]
```

If the user asks only for copy, provide copy only. If they ask for a carousel, include slide-by-slide copy plus a visual brief. If they ask for a paid campaign, include campaign objective, audience, creative, and measurement plan.

## CTA Rules

Use low-friction CTAs for organic posts:

- "Comment 'audit' and I will send the checklist."
- "DM me 'fleet' if you want the diagnostic template."
- "If this is happening in your operation, send me a note."
- "I can review one dashboard or maintenance workflow and tell you where value is leaking."

Use direct CTAs for paid ads:

- Book a diagnostic call
- Download checklist
- Request assessment
- Get roadmap

Avoid hype language such as "revolutionary", "guaranteed", "10x", "secret formula", or "limited time" unless the user explicitly requests a more aggressive direct-response style.

## Voice

Write in a grounded executive voice:

- Specific, practical, and slightly contrarian
- Confident without bragging
- Warm but not casual
- Technical enough to be credible, simple enough for executives
- Prefer mining and operations language over marketing language

Good phrases:

- "The issue is rarely lack of data. It is lack of operating rhythm."
- "Technology only creates value when it changes decisions."
- "A dashboard is not a transformation plan."
- "Maintenance performance is a business system, not a department metric."
- "The fastest way to improve reliability is often to fix planning, accountability, and decision cadence before buying more software."

Avoid:

- Generic hustle language
- Overly inspirational quotes
- Empty AI buzzwords
- Claims that sound like a vendor pitch
- Long paragraphs on carousel slides

## Research Workflow

When the user wants inspiration, competitor research, or examples:

1. Use Firecrawl MCP for page extraction when the source is crawlable.
2. Use Playwright MCP for JavaScript-heavy pages, menus, search pages, or visible result extraction.
3. Summarize patterns, do not copy ads or designs.
4. Create original offers, headlines, and layouts.

For LinkedIn-specific research, avoid scraping private or login-gated data. Use public pages, user-provided files, or user-provided examples.

## Production Workflow

When the user wants files created:

- Pair this skill with `adolfo-linkedin-brand-system` when the output is for Adolfo Salas, GoalPraxis, mining advisory, asset performance, AI/BI for mining, or personal-brand service offers. This skill defines the offer/copy/CTA; `adolfo-linkedin-brand-system` defines the visual identity and production rules.
- Pair this skill with `linkedin-multiformat-generator` when the user wants one campaign transformed into all LinkedIn formats (text, single image, carousel, lead magnet, infographic, GIF, MP4/video).
- Use Slidev for fast editable carousel-style decks.
- Use PPTX when the user wants business-editable slides.
- Use canvas/static design tools for one-page posters or ad images.
- Use frontend design skills for landing pages or visual prototypes.
- Keep text editable whenever possible.

Default deliverables:

- Markdown strategy/copy file
- Slidev or PPTX carousel source
- PDF export for LinkedIn upload
- PNG/JPG single-image ad variant when requested

## Quality Checklist

Before finalizing, verify:

- The offer names a clear buyer and pain.
- The hook creates curiosity without clickbait.
- Each carousel slide has one idea.
- The CTA asks for one action.
- The copy includes proof or lived experience.
- Claims are credible and not exaggerated.
- The language sounds like an experienced operator-advisor, not a generic marketer.
- The format fits LinkedIn mobile viewing.

## Quick Prompts This Skill Should Handle

- "Create a LinkedIn carousel to sell my mining asset performance advisory service."
- "Make 5 LinkedIn ad angles for GoalPraxis."
- "Turn this service into a LinkedIn paid ad and organic post."
- "Create a PDF carousel offer for predictive maintenance consulting."
- "Research these competitor ads and make original LinkedIn offer concepts."
- "Build me a lead magnet post for mining operators."

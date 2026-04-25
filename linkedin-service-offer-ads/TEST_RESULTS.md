# LinkedIn Service Offer Ads - Test Results

Date: April 24, 2026

## Iteration 1

Workspace:
`C:\Users\USER\.copilot\skills\linkedin-service-offer-ads-workspace\iteration-1`

## Tests Run

1. Mining advisory carousel
   - Prompt: Create a LinkedIn carousel to offer my mining asset performance advisory service to COOs and maintenance leaders.
   - Output: `eval-1-mining-advisory-carousel/with_skill/outputs/result.md`
   - Result: Passed structural check.
   - Word count: 708

2. GoalPraxis AI/BI angles
   - Prompt: Make 5 LinkedIn ad angles for GoalPraxis focused on AI-enabled business intelligence for mining operations.
   - Output: `eval-2-goalpraxis-ai-bi-angles/with_skill/outputs/result.md`
   - Result: Passed structural check.
   - Word count: 502

3. Predictive maintenance ad
   - Prompt: Turn my predictive maintenance consulting offer into a single-image LinkedIn ad and an organic text post.
   - Output: `eval-3-predictive-maintenance-ad/with_skill/outputs/result.md`
   - Result: Passed structural check.
   - Word count: 402

## Observations

- The skill produced the intended LinkedIn service-offer structures.
- The outputs used a grounded mining operator-advisor voice.
- The outputs avoided unsupported guarantees and generic marketing hype.
- The subagent test environment could read the skill but could not write files directly, so final test artifacts were saved from the main session.

## Recommended Next Improvement

Run a second qualitative test by generating a real publish-ready carousel or ad package, then tune the skill based on tone preference and actual LinkedIn publishing workflow.

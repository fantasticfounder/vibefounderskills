---
name: competitor-scan
description: "Lightweight competitor analysis for solo founders. Maps 5-7 competitors, applies simplified Porter's Five Forces, builds a value curve, and identifies the gap where you win. Triggers: competitor analysis, competitor research, competitive landscape, who are my competitors, what else exists, competitive scan."
---

# Competitor Scan

A focused competitive scan - not a 50-page MBA report. Just enough to know what you're up against and where you win.

## Context

You are helping a vibecoder understand the competitive landscape for: **$ARGUMENTS**.

If running in sequence from /discover-customers, use the target audience identified in the find-target-audience step to scope the competitive analysis to that specific segment.

## Why This Matters

Most vibecoders either ignore competitors entirely ("I'll just build something better") or obsess over them ("They have 10 million users, I can't compete"). Both are wrong.

The goal is not to copy or fear competitors. The goal is to understand the landscape well enough to find the GAP - the underserved need, the overlooked audience, the feature nobody else bothered to build. That gap is where you win.

## Instructions

> Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These apply throughout this skill.

### Step 1: Gather Existing Knowledge

Ask what the founder already knows:
- "Who do you know of that does something similar?"
- "What alternatives do your users (or potential users) currently use?"
- "Have you looked at any competitor products? What did you notice?"

Don't assume zero knowledge. Many founders have already done informal research. Build on it.

### Step 2: Map the Competitive Landscape

Use web search to find competitors across four categories:

**Direct competitors** - products that do roughly the same thing for roughly the same audience:
- Search: `"[product type] for [audience]"`, `"best [product type]"`, `"[product type] tool"`
- Check ProductHunt, G2, Capterra for the product category

**Indirect competitors** - products that solve the same problem differently:
- Search: `"[product type] alternatives"`, `"[problem] solution"`
- Look for adjacent categories that serve the same need

**Manual/DIY alternatives** - how people solve this without a dedicated product:
- Spreadsheets, Notion templates, manual processes, hiring freelancers
- Search: `"[problem] spreadsheet template"`, `"[problem] how do you handle" site:reddit.com`

**The "do nothing" option** - the most dangerous competitor:
- What happens if people just live with the problem?
- How bad is "doing nothing" for this audience?

Aim for 5-7 total entries across all categories.

For each competitor, gather:

```
| Name | Type | What They Do | Who They Target | Pricing | Key Strength | Key Weakness |
|---|---|---|---|---|---|---|
| [name] | Direct/Indirect/DIY | [one sentence] | [audience] | [free/freemium/$X/mo] | [one thing they do well] | [one thing they do poorly or ignore] |
```

### Step 3: Simplified Porter's Five Forces

Apply Michael Porter's Five Forces framework ("Competitive Strategy", 1980) in a simplified form relevant to indie/micro-SaaS founders:

```markdown
### Competitive Forces Assessment

**1. Rivalry intensity**: [Low / Medium / High]
How crowded is this space? Are competitors actively fighting for the same customers, or is everyone carving out a niche?
- [Evidence: number of direct competitors, how similar they are, whether they compete on features vs price]

**2. Barrier to entry**: [Low / Medium / High]
How easy is it for someone else to build what you're building? (Hint: for vibecoders, the answer is usually "very easy" - which means your moat is NOT the product, it's the audience relationship, distribution, or data.)
- [Evidence: technical complexity, data requirements, network effects, switching costs]

**3. Substitute threat**: [Low / Medium / High]
How easily can people solve this problem WITHOUT a dedicated product? (Spreadsheets, manual processes, hiring someone)
- [Evidence: DIY alternatives found, how good they are, what they cost in time/money]

**4. Buyer power**: [Low / Medium / High]
How much leverage do customers have? Can they easily switch between competitors? Are there many alternatives?
- [Evidence: switching costs, number of alternatives, price sensitivity]

**5. Overall competitive pressure**: [Low / Medium / High]
Bottom line: is this a market where a solo founder with a focused product can win?
- [One-sentence assessment]
```

### Step 4: Build a Value Curve

Based on Blue Ocean Strategy (W. Chan Kim and Renee Mauborgne, "Blue Ocean Strategy", 2004), create a value curve comparing the founder's product against the top 3 alternatives.

Choose 5-7 factors that matter to the target audience. These should be things customers actually evaluate when choosing a product - not internal technical metrics.

Good factors: ease of use, price, speed, customisation, integrations, support quality, mobile experience, learning curve, feature depth
Bad factors: code quality, tech stack, server uptime (customers don't evaluate these)

```
### Value Curve

Factors rated 1 (Low) to 5 (High):

| Factor | Your Product | [Competitor 1] | [Competitor 2] | [Competitor 3] |
|---|---|---|---|---|
| [Factor 1] | X | X | X | X |
| [Factor 2] | X | X | X | X |
| [Factor 3] | X | X | X | X |
| [Factor 4] | X | X | X | X |
| [Factor 5] | X | X | X | X |
```

If the founder's product scores the same as competitors on every factor, they have no differentiation. The goal is to find factors where they score HIGHER than everyone else, and factors they can deliberately score LOWER on (because their audience doesn't care about them).

### Step 5: Identify the Gap

This is the payoff. Based on the landscape, Five Forces, and value curve, answer:

1. **Where do you win?** - What does your product do (or could do) that competitors don't cover, don't care about, or do poorly?
2. **Who do competitors ignore?** - Is there an audience segment that no competitor specifically targets?
3. **What's the positioning opportunity?** - Based on the gap, how should you position against the competition? (Not "we're better" - that's not positioning. "We're the [product type] for [specific audience] who need [specific thing]" - that's positioning.)

## Output

Save as `[product-slug]-competitor-scan.md`. The report should include:

1. Competitive landscape table (5-7 entries)
2. Simplified Five Forces assessment
3. Value curve comparison
4. "Your gap" section with positioning opportunity
5. Key takeaways (3-5 bullet points)

```
---
Want the case studies and deep frameworks behind this?
fantasticfounder.com/join (free newsletter + paid membership)

Built by FantasticFounder - business strategy for vibecoders.
```

## Common Mistakes

- **Only looking at direct competitors.** The biggest threat to your app might not be another app - it might be a spreadsheet template that's "good enough."
- **Competing on features.** As a solo founder, you will never win a feature war against a funded startup. Compete on focus, speed, simplicity, or audience understanding instead.
- **Copying the leader.** If you build exactly what the market leader has but smaller, why would anyone switch? Differentiate or die.
- **Ignoring the "do nothing" option.** If the problem isn't painful enough for people to actively seek solutions, you're competing against apathy. That's the hardest competitor to beat.
- **Getting paralysed by competition.** Competition proves demand exists. Zero competitors often means zero demand. The question is not "do competitors exist?" but "is there a gap?"

## Notes

- This scan takes 10-20 minutes depending on market complexity
- It's designed for solo founders and micro-SaaS, not enterprise market analysis
- When running as part of /discover-customers, carry the landscape table and gap analysis forward into the demand-signals skill
- If the competitive pressure is High with no clear gap, recommend the founder reconsider their audience (go back to find-target-audience) or reposition (use ff-positioning plugin if available)

**Framework attribution**: Porter's Five Forces from Michael Porter, "Competitive Strategy" (1980). Blue Ocean Strategy and value curve from W. Chan Kim and Renee Mauborgne, "Blue Ocean Strategy" (Harvard Business Review Press, 2004). See CONVENTIONS.md for full attribution table.

---

### Further Reading

- [Understanding Your Competitors Without Obsessing Over Them](https://fantasticfounder.com) - Lightweight competitive analysis that helps you differentiate instead of copy

---
name: find-niche
description: "Find your niche when you can build anything but don't know who for. Combines market opportunity analysis with founder-market fit to identify niches with real demand and low competition. Triggers: find niche, what niche, who should I target, niche selection, pick a market, choose a niche, niche down."
---

# Find Your Niche

You can build anything. That's the problem. This skill helps you find a specific niche where demand exists, competition is low, and you have an unfair advantage.

## Context

You are helping a founder find their niche for: **$ARGUMENTS**.

If the user provides skills, interests, market research, or ideas they've considered, read those first.

## Why Niche Selection Matters

The paradox of choice: the more you CAN build, the harder it is to decide WHAT to build. Builders who pick a clear niche outperform generalists because:

1. **Specific messaging converts better.** "Invoice tool for freelance designers" beats "Invoice tool for everyone" - every time.
2. **Smaller ponds are easier to dominate.** Being the #1 tool for a niche of 5,000 people is more achievable and profitable than being the #500 tool in a market of millions.
3. **Niches have communities.** Specific audiences congregate in specific places. Targeting "small businesses" means targeting nowhere. Targeting "Shopify store owners doing $10K-50K/month" means you know exactly where they are (r/shopify, Shopify forums, ecommerce Twitter).
4. **Word of mouth travels faster in niches.** People in tight communities talk. One happy user can refer five others.

## Instructions

Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These apply throughout this skill.

### Step 1: Map Your Assets

Before looking at markets, look at what you bring:

**Skills inventory:**
- What technical skills do you have? (languages, frameworks, platforms)
- What non-technical skills? (design, writing, sales, domain expertise)
- What have you built before?

**Domain knowledge:**
- What industries have you worked in?
- What communities are you part of?
- What problems have you experienced personally?
- What topics do you naturally read about or follow?

**Access and network:**
- Who do you know? (potential first users, experts, distribution partners)
- What communities are you already a member of?
- What platforms do you already have presence on?

**Founder-market fit is an unfair advantage.** A fitness coach who codes has founder-market fit for fitness SaaS. A freelancer who codes has founder-market fit for freelancer tools. Don't ignore this.

When generating niche candidates in Step 2, explicitly cross-reference each candidate against your assets from Step 1. A niche that leverages 3+ of your assets has stronger founder-market fit.

### Step 2: Generate Niche Candidates

Combine your assets with market patterns. Use these niche generation methods:

**Method 1: Audience + Problem**
Pick a specific audience from your network/experience, then find their top 3-5 problems.
- Example: "I know freelance designers. Their problems: invoicing, project tracking, client communication, portfolio management, contract creation."

**Method 2: Platform + Gap**
Pick a platform your audience uses, then find what's missing or underserved.
- Example: "Shopify store owners have hundreds of analytics apps, but none of them explain what to DO with the data."

**Method 3: Keyword Demand Signals**
Use search data to find niches where people are searching but solutions are weak.
- Search Google for "[product type] for [audience]". If the first-page results are dominated by exact-match products, demand exists but competition is high. If Reddit threads, forums, or generic articles appear, demand exists but is underserved. If nothing relevant appears, demand is weak or the language is wrong.
- Example: "[tool type] for [audience]" keywords that show up with wide-open SERPs

**Method 4: Porter's Generic Strategies (Adapted)**
Michael Porter identified three competitive strategies in "Competitive Strategy" (1980). For niche selection, focus on one:
- **Cost leadership**: Build the cheapest version (race to bottom - usually bad for solo founders)
- **Differentiation**: Build the BEST version for a specific need (quality, features, experience)
- **Focus (niche)**: Build exclusively for one segment that's ignored by bigger players

For solo founders, **Focus** is almost always the right strategy. You win by being the ONLY option for a specific group, not by being a slightly cheaper/better option for everyone.

**Method 5: Blue Ocean Thinking**
From "Blue Ocean Strategy" by W. Chan Kim and Renee Mauborgne (2004). Instead of competing where everyone else is (red ocean), look for spaces where nobody is competing:
- What do competitors over-serve? (features nobody needs)
- What do competitors under-serve? (needs nobody addresses)
- What groups do competitors ignore? (audiences too small for big companies but perfect for solo founders)

Generate 5-10 candidate niches.

### Step 3: Evaluate Each Niche

Score candidates on 6 factors:

| Factor | 1 (Weak) | 3 (Moderate) | 5 (Strong) |
|---|---|---|---|
| **Demand signal** | No search volume, no communities discussing this | Some search activity, people asking questions | Clear BOFU keywords, people actively seeking solutions |
| **Competition** | Dominant incumbents with deep features and loyal users | Some players but none fully satisfying the niche | Few or no products specifically targeting this niche |
| **Willingness to pay** | Culture of free tools, no precedent for paying | Some paid tools exist, price sensitivity is moderate | Clear precedent for paying, strong ROI justification |
| **Founder-market fit** | No domain knowledge, no network, no personal experience | Some knowledge or adjacent experience | Deep domain expertise, existing network, personal pain |
| **Reachability** | Audience is scattered, no clear gathering points | Some communities exist, mixed with other audiences | Concentrated in specific communities, easy to target |
| **Growth potential** | Static market, no expansion path beyond niche | Moderate growth, some adjacent segments | Growing market, clear expansion path to adjacent niches |

When scores tie, prioritise: (1) Demand signal and Willingness to pay (these are verifiable with evidence), (2) Founder-market fit (hard to fake), (3) Growth potential (speculative - use as tiebreaker only).

### Step 4: Validate the Top 2-3

For the highest-scoring niches, do quick validation:

1. **Search check**: Run key product-type keywords through Google. Are the SERPs wide open or locked up? (Use validate-idea skill for deeper analysis)
2. **Community check**: Find 2-3 communities for this niche. Are people discussing the problem? Are existing solutions criticised?
3. **Competitor check**: Who already serves this niche? How well? What are the gaps?
4. **Revenue check**: Are there paid products in this space? What do they charge? What does the pricing tell you about willingness to pay?

### Step 5: Output the Niche Analysis

```
## Niche Analysis: [Your Area of Focus]

**Date**: [today]
**Founder skills**: [summary of relevant skills/experience]

### Candidate Niches

| # | Niche | Demand (1-5) | Competition (1-5) | WTP (1-5) | Founder Fit (1-5) | Reachability (1-5) | Growth (1-5) | Total (/30) |
|---|---|---|---|---|---|---|---|---|
| 1 | [niche] | [score] | [score] | [score] | [score] | [score] | [score] | [total] |
| 2 | [niche] | [score] | [score] | [score] | [score] | [score] | [score] | [total] |
| ... | ... | ... | ... | ... | ... | ... | ... | ... |

### Top Niche Validation

**Niche 1: [name]**
- Search demand: [what BOFU keywords exist, SERP accessibility]
- Communities: [where this audience congregates]
- Competitors: [who serves them now, what's missing]
- Revenue evidence: [what people pay for similar tools]
- Expansion path: [adjacent niches to grow into]

**Niche 2: [name]**
- [same structure]

### Recommendation

**Best niche**: [specific niche]
**Why**: [2-3 sentence justification covering demand, competition, and founder fit]
**Competitive strategy**: [Focus/Differentiation - how to win]

### Next Steps
1. Validate demand with keyword research (validate-idea skill)
2. Define your positioning within this niche (positioning-canvas skill)
3. Identify your beachhead segment within the niche (beachhead-segment skill)
```

Save as markdown.

## Common Mistakes

- **Picking a niche because it's big, not because you can win.** "AI tools" is huge and impossible to win. "AI writing assistant for legal briefs" is specific and winnable.
- **Ignoring founder-market fit.** Building for an audience you don't understand means slower learning, weaker messaging, and more wrong assumptions.
- **Niching too broadly.** "Small businesses" is not a niche. "Shopify store owners doing $10K-50K/month who need inventory forecasting" is a niche.
- **Niching too narrowly.** A meditation timer app that only targets Buddhist monks in rural Thailand - the market is too small and too hard to reach digitally. Your niche needs at least a few hundred potential customers.
- **Analysis paralysis.** Perfect niche selection doesn't exist. Pick the best of your options and validate fast. You can pivot niches in 2-4 weeks if the data says to.

## Notes

- This skill is about choosing WHERE to compete. The positioning-canvas skill defines HOW to compete within that niche.
- Niche selection and idea validation are complementary. Niche first, then validate specific product ideas within that niche.
- Revisit your niche every quarter as you learn from customers and the market evolves.

---

### Further Reading

- [How to Find Your Niche When You Can Build Anything](https://fantasticfounder.com) - Niche selection framework for vibecoders drowning in possibilities

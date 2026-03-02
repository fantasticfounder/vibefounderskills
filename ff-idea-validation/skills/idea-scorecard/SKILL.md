---
name: idea-scorecard
description: "Score a product idea on a 0-1.0 scale using 7 evidence-based demand factors. Turns gut feeling into a confidence number. Use when you've done some keyword research and want to objectively compare ideas. Triggers: score my idea, idea score, demand confidence, compare ideas, which idea is better, rate my idea."
---

# Idea Scorecard

Score your product idea on a 0-1.0 scale using keyword demand evidence. No gut feeling, no vibes - just data.

## Context

You are scoring the idea: **$ARGUMENTS**.

If the user provides keyword research, SERP analysis, or competitor data, use that. Otherwise, help them gather the evidence first (suggest using validate-idea or keyword-demand-check skills).

## Instructions

> Read CONVENTIONS.md for web search policy, DA proxy rules, and search volume proxies. These apply throughout this skill.

### Step 1: Gather Evidence

You need evidence for 7 factors. Ask the user what they already know. If the user has not run validate-idea or provided keyword research, recommend they do so first. This scorecard requires evidence, not estimates.

### Step 2: Score Each Factor

Score each factor on a 0-2 scale:

| Factor | Weight | Score 2 (Strong) | Score 1 (Present) | Score 0 (Absent) |
|---|---|---|---|---|
| **BOFU keyword count** | 3x | 10+ BOFU keywords found | 5-9 BOFU keywords | Fewer than 5 |
| **Solution-language presence** | 3x | 50%+ of keywords contain tool/template/app/etc | 20-49% contain solution words | Fewer than 20% |
| **Wide-open SERPs** | 2x | 50%+ of BOFU keywords have wide-open SERPs | 20-49% are wide open | Fewer than 20% |
| **Problem-aware searches** | 2x | Problem keywords exist with 500+ total monthly volume | 100-499 total volume | Below 100 total |

> **Note on Factor 4**: If the user has no keyword tool data for search volume, use the proxy rules from CONVENTIONS.md (Google autocomplete, "People also ask" boxes, Reddit thread density) and flag it: "Volume estimated via proxies - not tool-verified."
| **Commercial intent** | 1x | Keywords include buy/free/pricing/download/compare/vs/alternative/best | Some commercial modifiers | None |
| **SERP accessibility** | 2x | Top 5 results are mostly low-authority sites (personal blogs, forums, thin content, unrecognised domains) | Top 5 are a mix of medium-authority sites (established niche blogs, mid-size SaaS) | Top 5 are dominated by high-authority household brands (Forbes, Shopify, Google, Amazon, Wikipedia) |
| **Keyword clustering** | 1x | Keywords cluster into 5+ distinct page topics | 3-4 clusters | Fewer than 3 |

### Step 3: Calculate the Score

**Maximum possible raw score**: (3x2) + (3x2) + (2x2) + (2x2) + (1x2) + (2x2) + (1x2) = 28

**Demand Confidence Score** = your raw score / 28, rounded to one decimal place.

### Step 4: Interpret the Result

| Band | Score | What It Means | What to Do |
|---|---|---|---|
| **Weak** | 0.1 - 0.4 | Few or no BOFU keywords. SERPs are competitive or irrelevant. People aren't searching for this. | Park the idea. Try a different niche or product type. Don't invest time or money. |
| **Moderate** | 0.5 - 0.7 | Some signals but unclear. BOFU keywords exist but SERPs are competitive, or volume is very low. | Investigate more. Try repositioning with idea-flip. Spend 30-60 more minutes exploring. If it doesn't improve, park it. |
| **Validated** | 0.7 - 0.85 | Multiple BOFU keywords with accessible SERPs. Solution language present. Real demand confirmed. | Build it. Start with a landing page or MVP. |
| **Strong** | 0.85 - 1.0 | Wide-open BOFU keywords, low-DA SERPs, solution language everywhere, strong clustering. Rare. | Build it NOW. This is a high-priority opportunity. Move fast before someone else targets these keywords. |

### Step 5: Output the Scorecard

```
## Demand Confidence Scorecard: [Idea Name]

**Idea**: [one-sentence description]
**Date**: [today]

| Factor | Weight | Evidence | Score |
|---|---|---|---|
| BOFU keyword count | 3x | [what you found] | [0/1/2] |
| Solution-language presence | 3x | [what you found] | [0/1/2] |
| Wide-open SERPs | 2x | [what you found] | [0/1/2] |
| Problem-aware searches | 2x | [what you found] | [0/1/2] |
| Commercial intent | 1x | [what you found] | [0/1/2] |
| SERP accessibility | 2x | [what you found] | [0/1/2] |
| Keyword clustering | 1x | [what you found] | [0/1/2] |

**Raw Score**: [X] / 28
**Demand Confidence Score**: [X.X]
**Band**: [Weak / Moderate / Validated / Strong]

### Recommendation
[Clear recommendation based on the score]

### Key Strengths
- [What's working for this idea]

### Key Risks
- [What's concerning]

### Next Steps
- [What to do next based on the score]
```

Save as markdown.

## Scoring Discipline

- Do NOT inflate scores to be encouraging. If evidence is missing, score 0.
- The average idea should score 0.4-0.6. Most ideas are moderate at best.
- Justify every score with keyword evidence, not gut feeling.
- If comparing ideas, score each independently before comparing.

---

### Further Reading

- [The Idea Validation Checklist: Score Your App Idea Before You Build It](https://fantasticfounder.com) - A systematic scoring framework so you stop guessing whether your idea has legs

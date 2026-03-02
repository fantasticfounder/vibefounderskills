---
name: product-name
description: "Brainstorm product names aligned to your positioning and target audience. Evaluates names on memorability, domain availability, SEO impact, and brand fit. Triggers: name my product, product name, what should I call it, app name, brand name, naming, rename."
---

# Name Your Product

Brainstorm product names that are memorable, available, and aligned to how your product is positioned. A name doesn't make or break a product, but a good name makes everything else easier.

## Context

You are helping a founder name their product: **$ARGUMENTS**.

If the user provides positioning work, value propositions, target audience details, or name ideas they've already considered, read those first.

## What Makes a Good Product Name

**A good name is:**
- **Easy to say and spell.** If you have to spell it out every time, it's too complicated.
- **Easy to remember.** After hearing it once, can someone recall it a day later?
- **Relevant to the product's value or audience.** The name doesn't need to describe the product literally, but it should feel right in context.
- **Available.** Domain, social handles, and (ideally) trademark-clear.
- **Not easily confused with competitors.** If it sounds like a competitor, people will mix you up.

**A good name does NOT need to:**
- Describe exactly what the product does (Apple, Slack, Notion, Stripe - none describe the product)
- Be clever or punny (these age poorly and confuse international audiences)
- Use AI, GPT, Base, Hub, -ify, or -ly in the name (overused and undifferentiated as of 2025-2026)

## Instructions

Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These apply throughout this skill.

### Step 1: Define Naming Criteria

Based on the product and positioning, decide what the name should convey:

| Factor | Your Product |
|---|---|
| **Tone** | [Professional / Playful / Technical / Friendly / Bold / Minimal] |
| **Audience expectation** | [What do similar products in this space tend to be named?] |
| **Key association** | [What feeling or concept should the name evoke?] |
| **Naming style preference** | [Real word / Invented word / Compound / Acronym / Metaphor] |
| **Constraints** | [Must have .com? Must be under X characters? Language considerations?] |

### Step 2: Generate Name Candidates

Use 5 naming strategies. Generate 3-5 strong candidates per strategy. Quality over quantity. Do not generate names you wouldn't recommend.

**Strategy 1: Descriptive names**
Names that hint at what the product does.
- Take a key action or outcome and make it a name
- Examples: Grammarly (grammar), Mailchimp (mail), Buffer (social media buffer/queue)

**Strategy 2: Metaphor names**
Names that use a metaphor for the product's value.
- Think about what your product is LIKE
- Examples: Slack (easy communication), Notion (ideas/concepts), Basecamp (starting point)

**Strategy 3: Invented words**
Made-up names that are distinctive and ownable.
- Combine syllables, blend words, modify existing words
- Examples: Spotify, Figma, Vercel, Supabase. Indie/micro-SaaS examples: Plausible (analytics), Cal.com (scheduling), Tally (forms)

**Strategy 4: Real words (repurposed)**
Existing words used in a new context.
- Short, common words that feel fresh in your product context
- Examples: Stripe, Linear, Arc, Pitch, Craft

**Strategy 5: Compound names**
Two words combined into one name.
- Combine a concept + a modifier
- Examples: Airbnb (air + bed and breakfast), YouTube (you + tube), Dropbox (drop + box)

Generate 3-5 candidates per strategy.

### Step 3: Evaluate Each Name

Score candidates on 6 criteria (1-5 each):

| Criteria | 1 (Weak) | 3 (Moderate) | 5 (Strong) |
|---|---|---|---|
| **Memorability** | Forgettable, generic | Decent, but not distinctive | Sticks in your head after hearing it once |
| **Pronounceability** | Hard to say, unclear pronunciation | Manageable but not natural | Rolls off the tongue, obvious pronunciation |
| **Spellability** | Hard to spell, multiple possible spellings | Some ambiguity | No confusion, easy to type |
| **Relevance** | No connection to product or audience | Loose connection | Feels right for the product and audience |
| **Distinctiveness** | Sounds like existing products | Somewhat unique | Stands out, hard to confuse with competitors. Score by comparing against the top 3-5 competitor names in this space. If the name sounds similar to an existing competitor, it scores 1-2 regardless of other qualities. |
| **Scalability** | Too specific (limits future growth) | Works for current product | Works as the company grows and adds products |

### Step 4: Check Availability

For the top 3-5 names, check:
- **Domain**: Is [name].com available? What about [name].io, [name].app, [name].co?
- **Social handles**: Available on Twitter/X, GitHub, LinkedIn?
- **App stores**: Is the name taken on App Store / Play Store?
- **Trademark**: Any obvious conflicts? (Quick search, not legal advice)

Use web search to check domain and social handle availability. Web search cannot confirm domain registration status. Check if a live website exists - but a parked or blank domain may still be registered. Advise the founder to verify at namecheap.com, Google Domains, or similar before committing to a name.

### Step 5: Output the Name Recommendations

```
## Product Naming: [Product Description]

**Date**: [today]
**Positioning**: [one-sentence positioning]
**Tone**: [target tone]

### Naming Criteria
| Factor | Target |
|---|---|
| Tone | [tone] |
| Key association | [what it should evoke] |
| Style | [preferred naming style] |
| Constraints | [requirements] |

### Name Candidates

| # | Name | Strategy | Memo (1-5) | Pronounce (1-5) | Spell (1-5) | Relevance (1-5) | Distinct (1-5) | Scale (1-5) | Total (/30) |
|---|---|---|---|---|---|---|---|---|---|
| 1 | [name] | [strategy] | [score] | [score] | [score] | [score] | [score] | [score] | [total] |
| 2 | [name] | [strategy] | [score] | [score] | [score] | [score] | [score] | [score] | [total] |
| ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |

### Top 3 Recommendations

**1. [Name]** (Score: [X/30])
- Why it works: [rationale]
- Domain: [availability]
- Social handles: [availability]
- Potential concerns: [any issues]

**2. [Name]** (Score: [X/30])
- Why it works: [rationale]
- Domain: [availability]
- Social handles: [availability]
- Potential concerns: [any issues]

**3. [Name]** (Score: [X/30])
- Why it works: [rationale]
- Domain: [availability]
- Social handles: [availability]
- Potential concerns: [any issues]

### Final Recommendation
**Go with**: [name] - [one sentence why]
```

Save as markdown.

## Common Mistakes

- **Overthinking it.** A mediocre name with great positioning beats a great name with no positioning. Don't spend weeks naming. Spend hours.
- **Names that require explanation.** If you have to explain the name, it's not working. "Oh it's a play on words because..." - nobody cares.
- **Trend-chasing.** Don't add "AI" to the name just because AI is trendy. It dates your product and makes you generic.
- **Ignoring domain availability.** A brilliant name with no available domain is a practical nightmare. Check availability early.
- **Asking too many people.** Naming by committee produces bland names. Get 2-3 opinions, then decide.

## Notes

- Names can be changed later. Many successful products have been renamed (BackRub -> Google, Odeo -> Twitter). Don't let naming paralysis stop you from launching.
- This skill works best after positioning-canvas (which defines what the name needs to convey)
- The name is one piece of your brand. It works together with your positioning, visual design, and messaging.

---

### Further Reading

- [Naming Your App: A Decision Framework That Takes 30 Minutes](https://fantasticfounder.com) - Quick naming process for builders who want to ship, not deliberate

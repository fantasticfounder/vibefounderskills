---
name: assumption-check
description: "Identify the riskiest assumptions about your product idea before you invest time building. Finds what could go wrong across demand, usability, money, and feasibility. Use after validating demand to stress-test the idea. Triggers: what could go wrong, check my assumptions, risks, risky assumptions, stress test idea, will this fail, red flags."
---

# Check Your Assumptions

Every idea has hidden assumptions that can kill it. This skill finds them before you waste months building the wrong thing.

## Context

You are helping a vibecoder identify risky assumptions about their product: **$ARGUMENTS**.

If the user provides validation results, keyword data, or any research, read those first.

## Why This Matters

Vibecoders skip this step because building feels more productive than thinking. But the graveyard of failed apps is full of products where the builder assumed:
- "People will pay for this" (they won't)
- "People will find this" (they can't)
- "People will understand this" (they don't)
- "I can build this alone" (you can't - or it'll take 6 months)

Finding your riskiest assumption early saves you from building something nobody wants, can't use, won't pay for, or that you can't actually deliver.

## Instructions

> Read CONVENTIONS.md for web search policy, DA proxy rules, and search volume proxies. These apply throughout this skill.

### Step 1: Understand the Idea

Ask the user (if not already clear):
- What does the product do?
- Who is it for?
- How will people find it?
- How will you make money?

If they've already run validate-idea, use that data. Don't re-ask what you already know.

### Step 2: Identify Assumptions Across 4 Categories

Think about why this product might fail from four angles. For each category, list 2-4 specific assumptions the builder is making.

**1. Demand (Will anyone want this?)**
- Is anyone searching for this type of product?
- Is the problem painful enough that people actively look for solutions?
- Are there enough potential users to sustain a business?
- Is demand growing or shrinking?

**2. Usability (Will people figure it out?)**
- Can a first-time user get value within 5 minutes?
- Does the product require behaviour change or new habits?
- Is onboarding simple or complex?
- Will people stick with it after the first use?

**3. Money (Will it make money?)**
- Will people pay for this, or do they expect it to be free?
- Is the price you want to charge justified by the value?
- Can you acquire users for less than they'll pay you?
- Are there free alternatives that are "good enough"?

**4. Feasibility (Can you actually build and deliver this?)**
- Can you build this alone (or with your current resources)?
- Are there technical blockers (APIs, data sources, integrations)?
- Can you build a useful v1 in under 4 weeks?
- Will maintenance and support eat your time?

### Step 3: Rate Each Assumption

For each assumption, rate:

| Confidence | Meaning |
|---|---|
| **High** | You have evidence this is true (keyword data, user interviews, competitor success) |
| **Medium** | You believe it's true but haven't tested it |
| **Low** | You're guessing. No evidence at all. |

**What counts as "High confidence" evidence by category:**
- **Demand**: BOFU keywords found in validate-idea with accessible SERPs
- **Usability**: User tested a mockup with 3+ people and they completed the core task
- **Money**: Competitors charge this price and have paying customers
- **Feasibility**: Proof-of-concept for the hardest feature built and working

Also rate the impact if the assumption is WRONG:

| Impact | Meaning |
|---|---|
| **Critical** | If wrong, the entire product fails |
| **Significant** | If wrong, major pivot needed |
| **Minor** | If wrong, can adjust without major changes |

### Step 4: Identify the Riskiest Assumptions

The riskiest assumptions are: **Low confidence + Critical impact**.

These are the ones that need testing BEFORE you build. Flag the top 2-3.

### Step 5: Suggest Quick Tests

For each risky assumption, suggest a cheap, fast test:

| Assumption Type | Quick Tests |
|---|---|
| Demand | Search Google for BOFU keywords (validate-idea skill), check Reddit for people describing the problem, look for competitors |
| Usability | Show a mockup to 3 people, build a clickable prototype, do a 5-minute user test |
| Money | Check competitor pricing, ask 5 potential users "would you pay $X for this?", create a landing page with a price and measure clicks |
| Feasibility | Build the hardest feature first as a proof of concept, check API availability and limits, estimate build time honestly (then double it) |

### Step 6: Output the Assumption Map

```
## Assumption Map: [Product Name]

**Idea**: [one-sentence description]
**Date**: [today]

### Assumptions

| # | Category | Assumption | Confidence | Impact | Risk Level |
|---|---|---|---|---|---|
| 1 | Demand | [specific assumption] | [High/Med/Low] | [Critical/Significant/Minor] | [flag if risky] |
| 2 | Usability | [specific assumption] | [High/Med/Low] | [Critical/Significant/Minor] | [flag if risky] |
| ... | ... | ... | ... | ... | ... |

### Top 3 Riskiest Assumptions

1. **[Assumption]** - [Why it's risky + what happens if wrong]
2. **[Assumption]** - [Why it's risky + what happens if wrong]
3. **[Assumption]** - [Why it's risky + what happens if wrong]

### Recommended Tests

| Risky Assumption | Test | Effort | Time |
|---|---|---|---|
| [assumption] | [what to do] | [low/med/high] | [hours/days] |
| [assumption] | [what to do] | [low/med/high] | [hours/days] |
| [assumption] | [what to do] | [low/med/high] | [hours/days] |

### Overall Risk Assessment

**Riskiest area**: [Demand / Usability / Money / Feasibility]
**Recommendation**: [Test first / Proceed with caution / Rethink the approach]
```

Save as markdown.

## Scoring Discipline

- Don't rate everything as "medium" to avoid commitment. Be specific.
- If you have NO evidence for an assumption, it's Low confidence. Period.
- The most dangerous assumptions are the ones that feel so obvious you don't question them. Question them.
- Keyword data from validate-idea counts as evidence. "I think people want this" does not.

## Notes

- This takes 20-30 minutes per idea
- It pairs well with validate-idea (which tests demand assumptions) and pretotype-design (which designs tests for other assumptions)
- Solo founders should pay special attention to feasibility - you don't have a team to fall back on
- The goal is NOT to find reasons not to build. It's to find what to test FIRST so you build smarter.

---

### Further Reading

- [How to Test a Product Idea Without Building It](https://fantasticfounder.com) - Identify and test your riskiest assumptions before writing code

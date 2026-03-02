---
name: idea-flip
description: "Reposition your product idea when demand exists but your framing doesn't match how people search. Flips your idea into language customers actually use. Use when validate-idea shows weak BOFU keywords but strong problem keywords. Triggers: flip my idea, reposition idea, rebrand idea, idea not working, nobody searching for this, wrong framing, pivot idea."
---

# Flip Your Idea

Your product might be good - but your FRAMING might be wrong. This skill repositions your idea to match how real people actually search.

## Context

You are helping a vibecoder reposition their product idea: **$ARGUMENTS**.

If the user provides previous validation results, keyword data, or competitor research, read those first.

## When to Use This

You've validated your idea (using validate-idea or keyword-demand-check) and found:
- People search for the PROBLEM your app solves, but NOT for your type of product
- Your keywords are all "how to..." (top of funnel) with very few "tool for..." or "app for..." (bottom of funnel)
- The product is useful, but the words you use to describe it don't match what people type into Google

This is NOT about changing your product. It's about changing how you DESCRIBE it so it matches existing search behaviour.

## Instructions

> Read CONVENTIONS.md for web search policy, DA proxy rules, and search volume proxies. These apply throughout this skill.

Work through these steps. Be direct - if the idea can't be flipped after three attempts, say so.

### Step 1: Diagnose the Mismatch

Review the user's current idea framing and keyword data. Identify:

1. **What problem keywords exist?** (how to..., help with..., why does..., struggling with...)
2. **What solution keywords are missing?** (no "tool for...", "app for...", "template for..." results)
3. **What language gap exists?** The gap between the problem people describe and the product you want to build.

Summarise the mismatch clearly:
- "People search for [problem language], but nobody searches for [your product description]."

### Step 2: Apply the Four Flipping Rules

Try each rule in order. Stop as soon as one produces BOFU keywords.

**Rule 1: Find the Nearest Product Category**

If problem keywords exist but solution keywords don't, look for the nearest EXISTING product category that people already search for.

Ask: "What established product type is closest to what I'm building?"

Example:
- Your idea: "reading retention app" (nobody searches this)
- Nearest category: "book summary app" or "note-taking app" (thousands of searches)
- Flip: Position your product as a variant of the established category

**Rule 2: Use Words That Already Exist in Search Results**

If you can describe your product using a word that already appears in search results, use that word. Don't invent new categories - attach to existing ones.

Words that work: tool, template, tracker, planner, generator, checker, calculator, dashboard, app, software, platform, spreadsheet, kit, bundle.

Example:
- Your idea: "AI writing quality analyser" (no searches)
- Existing word: "grammar checker" (thousands of searches)
- Flip: Position as a grammar checker that does more

**Rule 3: Mine Customer Language from Communities**

If no product language exists at all, go to where your potential users talk about the problem:
- Reddit (subreddits relevant to the problem)
- X/Twitter (search the problem in quotes)
- Quora (questions about the problem)
- IndieHackers / Hacker News (for technical products)
- Facebook Groups (for consumer products)

**Search query templates**: Search `[problem description in plain English] site:reddit.com` and `"[core pain point]" site:reddit.com`. Search for the PROBLEM, not the product. Extract the EXACT phrases people use. These become new keyword seeds.

Example:
- Your idea: "team async communication tool"
- Reddit post: "I just need something that replaces our 47 Slack messages with one update per day"
- New seed: "daily standup tool", "async standup app", "Slack alternative for async teams"

Use web search to find these community discussions.

**Rule 4: The Three-Flip Limit**

If you've tried Rules 1-3 and STILL can't find BOFU keywords, the market may not be ready for this product.

After three repositioning attempts with no BOFU keywords:
- Park the idea
- Don't force it
- Try a completely different idea instead

Three flips is the limit. Beyond that, you're trying to create demand rather than capture it.

### Step 3: Validate the Flip

For each promising flip, do a quick SERP check:

1. Search Google for the new framing
2. Are there BOFU keywords? (tool/app/template + qualifier)
3. Are the SERPs accessible? (not all dominated by big brands)
4. Does the new framing still describe what your product actually does?

A good flip scores YES on all three. If the new framing doesn't describe your product, it's not a flip - it's a lie.

### Step 4: Output the Flip Report

```
## Idea Flip Report: [Original Idea]

**Original framing**: [what the user called their product]
**Problem**: [why the original framing doesn't match search behaviour]

### Flip Attempts

| # | New Framing | Rule Used | BOFU Keywords Found | SERPs Accessible | Viable? |
|---|---|---|---|---|---|
| 1 | [new framing] | [rule #] | [yes/no + examples] | [yes/no] | [yes/no] |
| 2 | [new framing] | [rule #] | [yes/no + examples] | [yes/no] | [yes/no] |
| 3 | [new framing] | [rule #] | [yes/no + examples] | [yes/no] | [yes/no] |

### Recommendation

**Best flip**: [which one, or "none - park this idea"]
**New positioning**: [one-sentence description using the flipped framing]
**Next step**: [validate the flipped idea with validate-idea, or try a different idea entirely]
```

Save as markdown.

## Common Mistakes

- **Flipping to something your product ISN'T.** The flip has to be honest. If your product is a meditation app, you can't flip it to "productivity tool" just because that keyword has volume. The product has to actually deliver what the keyword promises.
- **Flipping too broadly.** Going from "niche meeting timer" to "time management tool" is too broad. You'll rank for nothing. Stay specific.
- **Ignoring the flip data.** If all three flips fail, the answer is to try a different idea - not to flip a fourth time.
- **Only flipping the name, not the positioning.** The flip affects your landing page, your app store listing, your SEO, your pitch. It's not just a name change - it's a positioning change.

## Notes

- Idea flipping is a 15-30 minute exercise, not a week-long rebrand
- The best flips feel obvious in retrospect ("of course people search for grammar checker, not AI writing quality analyser")
- Many successful products are positioned as better versions of existing categories, not as new categories
- You're not "dumbing down" your product. You're making it findable.

---

### Further Reading

- [How to Find Product Market Fit When Your First Idea Doesn't Land](https://fantasticfounder.com) - Reframing techniques when your product is good but your positioning is wrong

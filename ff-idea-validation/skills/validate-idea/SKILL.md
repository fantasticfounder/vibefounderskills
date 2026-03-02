---
name: validate-idea
description: "Validate a product idea using search demand signals before building anything. Checks if real people are searching for what you want to build. Use when you have an app idea and want to know if there's demand. Triggers: validate idea, is my idea good, should I build this, idea validation, demand check, will people want this."
---

# Validate Your Idea

Check if real people want what you're thinking of building - using search behaviour as the primary signal.

## Context

You are helping a vibecoder validate their product idea: **$ARGUMENTS**.

If the user provides files (market research, competitor info, landing page), read them first. Use web search to understand the market if needed.

## Why This Matters

Most vibecoders build first, validate never. They ship an app in a weekend with Cursor or Replit, then wonder why nobody signs up. This skill flips the order: check demand BEFORE you build (or before you build MORE).

The core principle: **if people are searching for your type of product, demand exists. If they're not, it doesn't - no matter how cool your idea sounds.**

## Instructions

> Read CONVENTIONS.md for web search policy, DA proxy rules, and search volume proxies. These apply throughout this skill.

Work through these steps with the user. Be direct. If the idea has weak demand signals, say so.

### Step 1: Write the Idea Statement

Help the user write their idea as one sentence:

**"[Target audience] who want to [desired outcome] using [product type]."**

Examples:
- "Freelancers who want to send professional invoices using a simple web tool"
- "Fitness coaches who want to manage client bookings using a mobile app"
- "Small SaaS founders who want to understand their churn using an analytics dashboard"

If the idea is vague ("I want to build something with AI"), help them narrow it down. Ask:
- Who specifically would use this?
- What problem does it solve?
- What type of product is it? (tool, template, app, platform, marketplace)

### Step 2: Generate Keyword Seeds

Extract three types of seeds from the idea statement:

**Product-first seeds** - what the product IS:
- [product type] + [qualifier]: "invoice template free", "booking app for coaches", "churn analytics tool"

**Problem-first seeds** - what the user's PROBLEM is:
- [audience problem] + [solution word]: "track freelance income tool", "manage client schedule app", "why are users cancelling"

**Use-case seeds** - the product FOR a specific audience:
- [product type] + "for" + [audience/context]: "invoice tool for graphic designers", "booking system for personal trainers", "analytics for micro-SaaS"

Generate 15-30 seeds total. Use web search to check what language real people use when describing this problem. Search `[problem] site:reddit.com`, read top 5 thread titles and most upvoted comments, extract exact noun phrases people use. Also check forums and Quora for additional language patterns.

### Step 3: Classify by Search Intent

Tag each keyword:

- **BOFU (Bottom of Funnel)**: The searcher KNOWS they want a product and is looking for one. Keywords contain words like: tool, app, software, template, generator, platform, free, online, best, alternative, vs.
  - Example: "free invoice template for freelancers" = BOFU
- **MOF (Middle of Funnel)**: The searcher is comparing options.
  - Example: "FreshBooks vs Wave" = MOF
- **TOF (Top of Funnel)**: The searcher is just learning. They're NOT looking for a product.
  - Example: "how to invoice clients" = TOF

**Keep only BOFU and strong MOF keywords.** If you have fewer than 5 BOFU keywords, the idea may need repositioning (see the idea-flip skill).

### Step 4: Check Search Demand

For each BOFU keyword (or top 10 if you have more):

1. Search Google for the exact phrase
2. Note what's ranking:
   - Are the top results **product pages** (tools, apps, SaaS)? Good - this is a product SERP.
   - Are they **how-to articles** and blogs? Mixed signal - people search this but may not want a product.
   - Are they **Reddit threads** and forums? Great - Google has no good content, opportunity is wide open.
3. Note whether an **AI Overview** appears at the top. If it does, the keyword's opportunity drops one level (e.g., "Rankable" becomes "Competitive") because AI Overviews absorb clicks before users reach organic results.
4. Note the competition level using observable proxies (see CONVENTIONS.md for full DA proxy table):
   - **Wide open**: No page directly targets this keyword, mostly forums, personal blogs, and unrecognised domains
   - **Rankable**: Some targeting but from small/medium players, or no targeting but from established niche sites. Reddit threads taking positions.
   - **Competitive**: Direct targeting from established brands with dedicated product/landing pages
   - **Blocked**: All top results are from household-name brands (Google, Amazon, Shopify, Forbes, Wikipedia) - a new site cannot realistically rank here

### Step 5: Score the Idea

Use the keyword evidence to fill in this scorecard:

```
## Idea Scorecard: [Idea Name]

Total keyword seeds generated: [number]
Keywords classified as BOFU: [number]
Keywords classified as MOF: [number]
Wide open keywords: [number]
Rankable keywords: [number]
Competitive keywords: [number]
Blocked keywords: [number]

Solution-language keywords (containing tool/app/template/etc): [number]
Problem-language keywords (how to.../help with...): [number]

DEMAND SIGNAL: [STRONG / MODERATE / WEAK]
```

**Strong**: 10+ BOFU keywords, 50%+ wide open, solution language present
**Moderate**: 5-9 BOFU keywords, some wide open, mixed signals
**Weak**: Fewer than 5 BOFU keywords, most competitive/blocked, no solution language

### Step 6: Make a Recommendation

Based on the evidence:

- **Strong demand** -> "Your idea has real search demand. People are actively looking for this type of product. Build it."
- **Moderate demand** -> "There are signals, but they're not overwhelming. Try repositioning the idea (use /ff-idea-validation:idea-flip) or narrow your audience." Note: the idea-flip skill enforces a three-flip limit. If three repositioning attempts produce no BOFU keywords, recommend parking the idea.
- **Weak demand** -> "The search data doesn't support this idea. Either people don't search for this type of product, or the market is locked up by big players. Consider a different idea or a very different angle."

Be honest. Don't sugarcoat weak signals to be nice.

### Step 7: Save and Suggest Next Steps

Save the scorecard as a markdown file.

Then suggest:
- "Want me to **check specific keywords in depth**? Use the keyword-demand-check skill."
- "Want to **reposition this idea** to find better demand? Use the idea-flip skill."
- "Want to **identify what could go wrong** before you build? Use the assumption-check skill."
- "Ready to **test demand cheaply** before building the full product? Use the pretotype-design skill."

## Common Mistakes

- **Searching for YOUR product name instead of what customers would type.** You don't have a brand. Search for what a customer would type.
- **Only generating TOF keywords.** If all your seeds are "how to..." questions, you're thinking like a blogger, not a customer. Reframe: what would someone type when they already KNOW they want a tool?
- **Treating zero-volume keywords as zero demand.** Search tools underestimate long-tail volume. One keyword can deliver 5-10x the reported volume. But an idea supported ONLY by zero-volume keywords is a weaker signal.
- **Skipping the Google check.** Finding keywords is not validation. Validation is checking whether those keywords have accessible search results. An idea with 50 great keywords but all results blocked by Amazon and Google is NOT validated.
- **Falling in love with one idea.** This skill works best when you compare 2-3 ideas side by side.

## Notes

- This validation takes 30-60 minutes per idea
- It works for SaaS, tools, templates, digital products, marketplaces, and content businesses
- It does NOT work for products where demand doesn't express through search (pure viral products, social apps, games)
- The strongest signal is when you find BOFU keywords that are wide open - meaning people search for your product type and Google has nothing good to show them

**Framework attribution**: Keyword demand validation methodology based on Ed Sturm's Compact Keywords framework (2024-2025). See CONVENTIONS.md for full attribution table.

---

### Further Reading

- [How to Validate a Business Idea Before Writing a Single Line of Code](https://fantasticfounder.com) - Step-by-step validation process for vibecoders who build first and ask questions later

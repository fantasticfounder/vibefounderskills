---
name: keyword-demand-check
description: "Check if a specific keyword has real search demand and whether you can rank for it. Analyzes Google search results for competition level and opportunity. Use when you want to check a specific keyword before writing content or building a landing page. Triggers: keyword check, can I rank for, keyword research, search demand, SERP check, competition check."
---

# Keyword Demand Check

Check if a specific keyword has real demand and whether the search results are accessible to a new site.

## Context

You are checking search demand for: **$ARGUMENTS**.

Use web search to check Google for this exact phrase and analyze the results.

## Why This Matters

Most vibecoders skip this step entirely. They build a landing page targeting "AI productivity tool" without checking that Google's first page is dominated by Microsoft, Google, and Notion. Meanwhile, "AI meeting notes for freelancers" might be wide open.

**The principle: a keyword with 50 monthly searches and no competition beats a keyword with 5,000 searches and a wall of authority sites.**

## Instructions

> Read CONVENTIONS.md for web search policy, DA proxy rules, and search volume proxies. These apply throughout this skill.

### Step 1: Search Google

Search for the exact keyword phrase the user provided. Note:

1. **AI Overview**: Is there an AI-generated answer at the top? (Reduces clicks to organic results)
2. **Ads**: Are there paid ads? (Signals commercial value)
3. **Reddit/Forums**: Are Reddit threads, Quora answers, or forum posts ranking? (Signals Google is hungry for quality content)
4. **Top 5 organic results**: For each, note:
   - Site name and authority level (High/Medium/Low - see CONVENTIONS.md DA proxy table)
   - Whether the keyword appears in the page TITLE
   - Whether the keyword appears in the URL
   - Content type: product page, how-to article, listicle, tool page, or forum

### Step 2: Classify the SERP

Based on what you found:

| Classification | What It Means | Signal |
|---|---|---|
| **Wide Open** | No page directly targets this keyword. Top results are forums, personal blogs, unrecognised domains, or tangentially related pages. | Build a page targeting this keyword NOW. You can rank within weeks. |
| **Rankable** | Some targeting but from small/medium players (established niche blogs, mid-size SaaS), OR no targeting but from higher authority sites. Reddit threads taking positions. | Build this page. You can rank within 2-4 months with decent content. |
| **Competitive** | Direct targeting from established brands with dedicated product/landing pages and clear professional depth. Multiple real competitors. | Build this page only after your site has some authority. Not a first-page priority. |
| **Blocked** | Top results are all household-name brands (Shopify, Forbes, HubSpot, Google, Amazon, Wikipedia) directly targeting this keyword. | Do NOT target this keyword as a new site. Find a longer-tail variation. |

**AI Overview adjustment**: If an AI Overview appears for this keyword, downgrade the classification by one level (e.g., "Rankable" becomes "Competitive"). AI Overviews absorb clicks before users reach organic results, reducing the value of ranking.

### Step 3: Check Intent Alignment

Does the SERP match what you'd want to rank with?

- **Product SERP**: Top results are product/tool/service pages. If you're building a product, this is perfect.
- **Content SERP**: Top results are how-to articles and guides. If you're building a product, your landing page might not match what Google wants to show.
- **Mixed SERP**: Some product pages, some content. Worth targeting but test which format works.
- **List SERP**: Top results are all "best of" or "top 10" listicles. Harder to rank with a single product page.

### Step 4: Suggest Variations

If the keyword is competitive or blocked, suggest 3-5 longer-tail variations that might be more accessible:

- Add a qualifier: "free", "online", "no signup", "for [specific audience]"
- Add a use case: "for freelancers", "for small teams", "for solopreneurs"
- Add a comparison: "vs [competitor]", "alternative to [known tool]"
- Add a format: "template", "generator", "checker", "calculator"

Search for 1-2 of the most promising variations to verify they're actually more accessible.

### Step 5: Deliver the Verdict

```
## Keyword Check: "[keyword]"

**Classification**: [Wide Open / Rankable / Competitive / Blocked]
**Intent**: [Product / Content / Mixed / List]
**Recommendation**: [Build now / Build later / Don't target / Try variation]

### What's Ranking
1. [Site] - Authority: [High/Medium/Low] - [targets keyword? yes/no] - [content type]
2. [Site] - Authority: [High/Medium/Low] - [targets keyword? yes/no] - [content type]
3. [Site] - Authority: [High/Medium/Low] - [targets keyword? yes/no] - [content type]
4. [Site] - Authority: [High/Medium/Low] - [targets keyword? yes/no] - [content type]
5. [Site] - Authority: [High/Medium/Low] - [targets keyword? yes/no] - [content type]

**AI Overview present?** [Yes/No] [If yes, note impact on classification]

### Key Observations
- [Notable finding about the SERP]
- [Notable finding about competition]
- [Notable finding about opportunity]

### Suggested Variations (if competitive)
- "[variation 1]" - [likely classification]
- "[variation 2]" - [likely classification]
- "[variation 3]" - [likely classification]
```

## Tips

- Reddit threads ranking = strongest opportunity signal. Google literally doesn't have quality content to show.
- "People also ask" boxes reveal what related questions people search - mine these for more keywords.
- If a beauty magazine or completely unrelated site ranks for your keyword, the SERP is starving for relevant content.
- Keywords showing 0-10 monthly volume in tools like Moz can still deliver hundreds of clicks. Don't dismiss low-volume keywords if the SERP is wide open.

---

### Further Reading

- [How to Do Market Research for Your App in 30 Minutes](https://fantasticfounder.com) - Quick demand validation using free tools and search behaviour analysis

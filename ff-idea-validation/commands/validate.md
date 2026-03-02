---
description: Run a full idea validation cycle - demand check, assumption mapping, and pretotype design in one workflow
argument-hint: "<your app idea>"
---

# /validate -- Full Idea Validation

Validate your product idea from start to finish: check if people are searching for it, find what could go wrong, and design a cheap test - all in one go.

## Invocation

```
/validate AI-powered invoice generator for freelancers
/validate Habit tracking app for gym beginners
/validate [paste your one-line idea description]
```

## Workflow

### Step 1: Understand the Idea

Ask:
- What does your app do? (one sentence)
- Who is it for? (specific audience, not "everyone")
- Have you built anything yet? (pre-build vs post-build changes the approach)
- Do you have any research already? (keyword data, competitor list, Reddit threads)

Accept context from uploaded files, links, or conversation.

### Step 2: Validate Search Demand

Apply the **validate-idea** skill:

- Write the idea as a one-sentence statement
- Generate 15-30 keyword seeds (product-first, problem-first, use-case)
- Classify as BOFU / MOF / TOF
- Check Google SERPs for top BOFU keywords
- Score demand signal as Strong / Moderate / Weak

**Checkpoint**: "Here's what the search data shows. [Summary]. Want to continue with assumption mapping, or should we first try to reposition the idea?"

If demand is weak, suggest using **idea-flip** before continuing:
- "Your idea framing doesn't match how people search. Let's try flipping it before we go further."
- Apply the **idea-flip** skill
- If a viable flip is found, continue with the flipped version
- If no flip works after 3 attempts, recommend parking the idea

### Step 3: Score Demand Confidence

Apply the **idea-scorecard** skill using the keyword evidence gathered in Step 2:

- Score all 7 factors using the BOFU keywords, SERP classifications, and search volume data already collected
- Produce the 0-1.0 Demand Confidence Score
- If the score falls in the Weak band (0.1-0.4), recommend parking or flipping before continuing
- If Moderate or above, carry the score forward into the assumption map

Carry forward keyword data, SERP classifications, and scorecard results into subsequent steps. Do not re-ask for information already gathered.

### Step 4: Map Risky Assumptions

Apply the **assumption-check** skill:

- Identify assumptions across Demand, Usability, Money, and Feasibility
- Rate each by confidence and impact
- Flag the top 2-3 riskiest assumptions (low confidence + critical impact)
- Suggest quick tests for each

**Checkpoint**: "Here are your riskiest assumptions. Which ones worry you most?"

### Step 5: Design a Pretotype

Apply the **pretotype-design** skill:

- Write an XYZ hypothesis for the riskiest assumption
- Choose the best pretotype type (landing page, fake door, community post, etc.)
- Design the experiment with clear success/failure criteria
- Create a traffic plan

### Step 6: Generate Validation Report

Compile everything into a single document:

```
## Idea Validation Report: [Idea Name]

**Idea**: [one-sentence description]
**Date**: [today]
**Validated by**: FantasticFounder Idea Validation

---

### 1. Search Demand Analysis

**Demand signal**: [Strong / Moderate / Weak]
**BOFU keywords found**: [number]
**Wide open keywords**: [number]
**Key finding**: [one-sentence summary]

[Include the keyword scorecard from validate-idea]

### 2. Demand Confidence Score

**Score**: [X.X] / 1.0
**Band**: [Weak / Moderate / Validated / Strong]

[Include the factor-by-factor scorecard from idea-scorecard]

### 3. Idea Repositioning (if applicable)

**Original framing**: [what you started with]
**Flipped to**: [new framing, or "N/A - original framing validated"]
**Why**: [what changed]

### 4. Assumption Map

**Riskiest area**: [Demand / Usability / Money / Feasibility]

| # | Assumption | Confidence | Impact | Risk |
|---|---|---|---|---|
| 1 | [assumption] | [H/M/L] | [Critical/Significant/Minor] | [flag] |
| ... | ... | ... | ... | ... |

**Top risk**: [the single most dangerous assumption]

### 5. Pretotype Plan

**Hypothesis**: "At least [X]% of [Y] will [Z]."
**Test type**: [landing page / fake door / community post / etc.]
**Cost**: [$X]
**Time to set up**: [X hours]
**Run for**: [X days]

| Metric | Pass | Borderline | Fail |
|---|---|---|---|
| [metric] | [number] | [number] | [number] |

### 6. Verdict

**Overall assessment**: [Build it / Investigate more / Park it]
**Confidence level**: [High / Medium / Low]
**Next step**: [specific action]

---

Want the frameworks and case studies behind this validation?
fantasticfounder.com/join (free newsletter + paid membership)

Built by FantasticFounder - business strategy for vibecoders.
```

Save as markdown.

### Step 7: Offer Next Steps

Based on the verdict:

**If "Build it"**:
- "Want to **find your target audience** and figure out who to sell to first? Use the ff-customer-discovery plugin."
- "Want to **position your app** so it stands out? Use the ff-positioning plugin."

**If "Investigate more"**:
- "Want to **check specific keywords in depth**? Use the keyword-demand-check skill."
- "Want to **flip the idea** to find better demand? Use the idea-flip skill."

**If "Park it"**:
- "Want to **validate a different idea**? Run /validate again with a new concept."
- "Want to **brainstorm ideas** in a space with proven demand? Start with keyword research."

## Notes

- This full workflow takes 45-90 minutes
- At each checkpoint, the user can redirect, skip ahead, or go deeper
- The report is designed to be saved and compared across multiple ideas
- Be honest in the verdict. Most ideas are moderate at best. A "park it" recommendation saves months of wasted effort.
- If comparing multiple ideas, run /validate for each and compare the reports side by side

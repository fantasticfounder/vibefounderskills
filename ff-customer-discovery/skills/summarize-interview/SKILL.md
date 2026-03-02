---
name: summarize-interview
description: "Extract actionable insights from a customer interview transcript. Identifies JTBD, flags Mom Test violations, and pulls the one insight that should change what you build. Triggers: summarize interview, interview notes, interview summary, what did I learn, process interview."
---

# Summarize Interview

Turn a messy interview transcript into actionable insights - and flag the things you did wrong.

## Context

You are helping a vibecoder extract insights from a customer interview about: **$ARGUMENTS**.

The user will provide either a full transcript, voice recording notes, or rough interview notes. Work with whatever they have.

If this interview was conducted using a script from the customer-interview-script skill, the note-taking template may already be partially filled in. Use it as a starting point.

## Why This Matters

Most founders do interviews, nod a lot, feel good about the conversation, and then do nothing with the data. Or worse, they cherry-pick the one compliment and ignore the five warning signs.

This skill forces structured extraction. It separates signal from noise, flags where you accidentally pitched instead of listened, and identifies the one insight that should actually change your product or strategy.

## Instructions

> Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These apply throughout this skill.

### Step 1: Read the Full Transcript

Read everything the user provides. Don't skim. The most important insights are often buried in throwaway comments, not in direct answers to questions.

If the transcript is incomplete or unclear, ask:
- "What was the context for this interview? Who were you talking to?"
- "Were there any moments that surprised you?"
- "What was your gut feeling after the interview?"

### Step 2: Extract Structured Insights

Work through the transcript and pull out:

**Current solution**: What do they use today to handle this problem? Include manual processes, spreadsheets, competitors, workarounds, and "doing nothing."

**What works about it**: What do they genuinely like about their current approach? This tells you what NOT to break.

**What's broken**: Where does the current solution fail? Look for:
- Explicit complaints ("It's so frustrating when...")
- Workarounds ("So what I do is...")
- Time sinks ("I spend X hours per week on...")
- Emotional language ("I hate", "drives me crazy", "I wish")

Mark emotional intensity:
- Low: mild inconvenience, accepts it as normal
- Medium: actively annoyed, has looked for alternatives
- High: strong emotional language, has tried multiple solutions, spends significant time/money

**Jobs to Be Done** (Clayton Christensen, "Competing Against Luck", 2016):
- Functional job: What are they trying to get done?
- Emotional job: How do they want to feel?
- Social job: How do they want to be perceived by others?

**Willingness to pay signals**: Look for evidence, not opinions:
- Time invested in solving the problem (time = value)
- Money currently spent on alternatives
- Solutions they've already tried (each attempt = proof they care enough to act)
- Unprompted mentions of what they'd pay or invest

### Step 3: Flag Mom Test Violations

Review the transcript for places where the interview went off track. Based on Rob Fitzpatrick's "The Mom Test" (2013):

| Violation | What It Looks Like | Impact |
|---|---|---|
| **Pitched the product** | Founder explained what they're building, then asked for feedback | Responses after the pitch are unreliable - interviewee switched to polite mode |
| **Hypothetical questions** | "Would you use...?", "Would you pay...?" | Hypothetical answers predict nothing. Only past behaviour predicts future behaviour. |
| **Accepted compliments** | "That sounds great!" treated as positive signal | Compliments are social lubricant, not validation |
| **Leading questions** | "Don't you think it would be better if...?" | The answer was embedded in the question |
| **Future-tense questions** | "Will you...?", "How often would you...?" | People are terrible at predicting their own behaviour |

For each violation found, note:
- Where in the transcript it happened
- What reliable information was available before it went off track
- Whether any data gathered AFTER the violation can still be trusted

### Step 4: Identify the Key Insight

Find the ONE insight from this interview that should change what the founder builds or how they position it. This is usually:

- Something that contradicts the founder's assumptions
- An unexpected use case or need
- A pain point the founder didn't know about
- A competitor or alternative the founder hadn't considered
- Language the interviewee used that's different from how the founder describes their product

State it clearly: "The key insight from this interview is: [insight]. This matters because: [why it changes things]."

### Step 5: Generate Structured Summary

Output the following template, filled in with data from the transcript:

```markdown
## Interview Summary: [Product/Topic]

**Date**: [date of interview]
**Participant**: [name/code]
**Background**: [role, context, relevant details]

---

### Current Solution
[What they use today to handle this problem]

### What Works
[What they like about their current approach]

### What's Broken
[Pain points, with emotional intensity markers: LOW / MEDIUM / HIGH]

- [Pain point 1] - **[HIGH]** - "[exact quote if available]"
- [Pain point 2] - **[MEDIUM]** - "[exact quote if available]"
- [Pain point 3] - **[LOW]**

### Jobs to Be Done
(Clayton Christensen, "Competing Against Luck", 2016)

- **Functional**: [what they're trying to accomplish]
- **Emotional**: [how they want to feel]
- **Social**: [how they want to be perceived]

### Key Insight
[The one thing that matters most from this interview]

**Why this matters**: [how it should influence the product or strategy]

### Willingness to Pay
- Time spent on problem: [hours per week/month]
- Money spent on alternatives: [$X per month/year]
- Solutions already tried: [list]
- Direct signals: [any explicit mentions of value/price]

### Mom Test Violations
[List any violations found, or "None detected - clean interview"]

- [Violation type]: [where it happened and impact on data reliability]

### Action Items
- [ ] [Specific thing to do based on this interview]
- [ ] [Specific thing to do based on this interview]
- [ ] [Follow-up needed]
```

## Output

Save as `[product-slug]-interview-[participant-code].md`.

If the founder has done multiple interviews and wants a cross-interview synthesis, offer to run this skill on each transcript and then compile a pattern summary across all interviews.

```
---
Want the case studies and deep frameworks behind this?
fantasticfounder.com/join (free newsletter + paid membership)

Built by FantasticFounder - business strategy for vibecoders.
```

## Common Mistakes

- **Treating one interview as truth.** One person's experience is an anecdote. Wait until you see the same pattern across 3-5 interviews before treating it as a signal.
- **Ignoring the parts that contradict your thesis.** If someone says "I don't actually have this problem", that's data. Don't explain it away.
- **Over-indexing on compliments.** "I'd totally use that!" from someone who currently does nothing to solve the problem is noise. Actions speak louder than intentions.
- **Missing the emotional moments.** When someone's voice changes, when they lean forward, when they say "ugh" or "finally" - those are the real signals. Flag them.
- **Not tracking violations.** If you pitched your product halfway through, everything after that point is contaminated. Know which data you can trust.

## Notes

- Processing one transcript takes 5-10 minutes
- If the user has multiple transcripts, process each one separately, then offer to synthesize patterns
- When running as part of /discover-customers, feed insights from summaries into the user-personas skill
- This skill pairs directly with customer-interview-script: the note-taking template from that skill feeds into this one

**Framework attribution**: JTBD synthesis from Clayton Christensen, "Competing Against Luck" (2016). Mom Test violation framework from Rob Fitzpatrick, "The Mom Test" (2013). See CONVENTIONS.md for full attribution table.

---

### Further Reading

- [Turning Customer Conversations Into Decisions](https://fantasticfounder.com) - How to extract real insights from customer interviews instead of just feeling good about your idea

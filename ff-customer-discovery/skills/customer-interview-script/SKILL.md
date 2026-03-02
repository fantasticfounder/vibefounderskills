---
name: customer-interview-script
description: "Create a Mom Test-style interview script that surfaces real insights, not just compliments. Builds a complete interview guide with opening, context, core exploration, and wrap-up sections. Triggers: customer interview, interview script, interview questions, mom test, how to talk to customers, user interview, customer research questions."
---

# Customer Interview Script

Build an interview script that gets you real insights - not polite lies.

## Context

You are helping a vibecoder prepare for customer interviews about: **$ARGUMENTS**.

If the user has already identified a target audience (from the find-target-audience skill or their own research), use that to tailor the script. If running in sequence from the /discover-customers command, pull the primary target segment and mini-ICP from the previous step.

## Why This Matters

Most founders skip customer interviews entirely. The ones who don't usually do them wrong - they pitch their idea, ask hypothetical questions ("Would you use this?"), and collect compliments they mistake for validation.

Rob Fitzpatrick's "The Mom Test" (2013) fixes this. The core idea: **talk about their life, not your idea. Ask about the past, not the future. Listen more than you talk.** If you follow these rules, even your mom can't lie to you.

## Instructions

> Read CONVENTIONS.md for web search policy, context threading, and scoring conventions. These apply throughout this skill.

### Step 1: Define What You're Deciding

Before writing a single question, clarify what DECISION this research will inform. Interviews without a decision to make produce interesting-but-useless data.

Ask the founder:
- What decision are you trying to make? (Examples: "Which audience to focus on", "Whether to add feature X", "How to price this", "Whether people actually have this problem")
- What would change your mind? (If nothing would change their plan, interviews are a waste of time)
- How many interviews are you planning? (Minimum 5. Recommend 8-12 for patterns to emerge)

If the founder says "I just want to learn about my users" - push back. Learning without a decision is exploration, not research. Help them identify the specific question they need answered.

### Step 2: Build the Interview Script

Generate a complete script with four sections. Tailor all questions to the founder's product, audience, and decision.

```markdown
# Customer Interview Script: [Product/Topic]

**Decision this informs**: [what you're trying to decide]
**Target participant**: [who you're interviewing]
**Estimated time**: 25-30 minutes

---

## Section 1: Opening (2 minutes)

**Goal**: Build rapport, set expectations, get permission.

"Thanks for taking the time. I'm working on [general area - don't name your product yet] and trying to understand how people like you handle [problem area]. There are no right or wrong answers - I genuinely want to understand your experience. Would it be okay if I record this so I can focus on listening instead of note-taking?"

**Rules for this section:**
- Do NOT mention your product name or what it does
- Do NOT say "I built an app that..." - this triggers compliment mode
- Keep it under 2 minutes. You're here to listen, not explain.

---

## Section 2: Context (5 minutes)

**Goal**: Understand their world before diving into the problem.

"Walk me through your typical [day/week] when [problem area] comes up."

Follow-up questions:
- "How often does that happen?"
- "What does that look like in practice?"
- "Who else is involved when this comes up?"

**Rules for this section:**
- Let them set the frame. Their version of the problem may be different from yours.
- Note the language they use - these are your future marketing words.

---

## Section 3: Core Exploration (15-20 minutes)

**Goal**: Understand past behaviour, current pain, existing solutions, and willingness to pay.

### Past behaviour (the most reliable predictor of future behaviour):

- "Tell me about the last time you dealt with [problem]. What happened?"
- "What did you do about it?"
- "How did that work out?"

### Current solution:

- "What do you currently use to handle [problem area]?"
- "How did you find that solution?"
- "What do you like about it?"
- "What's frustrating about it?"
- "Have you tried anything else before this? What happened?"

### Pain intensity:

- "On a scale of 'minor annoyance' to 'I lose sleep over this', where does [problem] fall?"
- "What happens when [problem] goes unsolved? What's the real cost?"
- "Have you ever tried to solve this yourself? (Built a spreadsheet, wrote a script, hired someone?)"

### Willingness to pay:

- "Are you currently paying for anything to help with this?"
- "How much time do you spend on this per week/month?"
- "If you could wave a magic wand and this problem disappeared, what would that be worth to you?"

**Rules for this section:**
- Ask about PAST and PRESENT, never hypothetical futures
- When they say something interesting, use these probes:
  - "Tell me more about that."
  - "Why?" (ask up to 3 times to get to the real reason)
  - "Can you give me a specific example?"
  - "What happened next?"
- If they start giving you compliments ("That sounds cool!"), redirect: "I appreciate that, but I'm more interested in YOUR experience. Tell me more about how you handle [problem] today."

---

## Section 4: Wrap-Up (3 minutes)

**Goal**: Capture what you missed and get referrals.

- "Is there anything I should have asked about that I didn't?"
- "Is there anyone else you know who deals with this problem? Would you be comfortable introducing me?"
- "Would it be okay if I followed up with a quick question later if something comes up?"

"Thank you - this was genuinely helpful."

---
```

### Step 3: Add Mom Test Rules as Inline Reminders

Include these rules in the script as sidebar reminders the founder can reference during the interview:

```markdown
## Mom Test Rules (keep visible during interview)

Rob Fitzpatrick, "The Mom Test" (2013):

1. **Talk about their life, not your idea.** Bad: "I'm building an app that does X. Thoughts?" Good: "Tell me about the last time you dealt with [problem]."
2. **Ask about the past, not the future.** Bad: "Would you use a tool that does X?" Good: "What did you do the last time this happened?"
3. **Talk less, listen more.** If you're talking more than 30% of the time, you're pitching, not interviewing.
4. **Never pitch.** The moment you explain your product, the interview is over. They switch from honest mode to polite mode.
5. **Compliments are noise.** "That's a great idea!" means nothing. "I spent 3 hours last week doing this manually" means everything.
6. **Opinions are worthless. Behaviour is gold.** "I would definitely pay for that" = opinion. "I currently pay $50/month for a worse version" = signal.
```

### Step 4: Add Probing Techniques

Include a quick reference for going deeper:

```markdown
## Probing Techniques

When someone says something interesting, don't move to the next question. Go deeper:

- **"Tell me more about that."** - Opens the door without leading.
- **"Why?"** - Ask up to 3 times. The first answer is surface. The third answer is the real reason.
- **"Give me a specific example."** - Moves from abstract ("it's frustrating") to concrete ("last Tuesday I spent 2 hours...")
- **"What happened next?"** - Follows the story to its conclusion. Often reveals consequences the founder didn't anticipate.
- **"How did that make you feel?"** - Uncovers the emotional job. Use sparingly - people don't always articulate emotions well.

**Silence is a tool.** After they answer, wait 3 seconds before asking the next question. People often fill silence with their most honest thoughts.
```

### Step 5: Generate Note-Taking Template

```markdown
## Interview Notes Template

**Date**: ___________
**Participant name/code**: ___________
**Background**: ___________
**Channel found through**: ___________

### Key Observations

| Topic | What They Said (exact words) | My Interpretation |
|---|---|---|
| Current solution | | |
| What works about it | | |
| What's broken | | |
| Pain intensity | | |
| Time/money spent | | |
| Willingness to pay signals | | |

### Jobs to Be Done (Clayton Christensen, "Competing Against Luck", 2016)

- **Functional**: What are they trying to accomplish? ___________
- **Emotional**: How do they want to feel? ___________
- **Social**: How do they want to be perceived? ___________

### Strongest Moment

The most emotionally intense moment in the interview (strong language, frustration, excitement):

> [Quote them directly]

### Mom Test Violations

Did I accidentally:
- [ ] Pitch my product?
- [ ] Ask hypothetical questions ("Would you...")?
- [ ] Accept compliments as validation?
- [ ] Talk more than 30% of the time?
- [ ] Lead the witness with my questions?

### One Takeaway

The single most important thing I learned:

___________

### Follow-Up

- [ ] Send thank-you message
- [ ] Request intro to [name] they mentioned
- [ ] Follow up on [topic] in 1 week
```

## Output

Save the complete package as `[product-slug]-interview-script.md`. It should include:

1. The full 4-section interview script, tailored to the founder's product and audience
2. Mom Test rules sidebar
3. Probing techniques reference
4. Note-taking template (blank, ready to copy for each interview)

```
---
Want the case studies and deep frameworks behind this?
fantasticfounder.com/join (free newsletter + paid membership)

Built by FantasticFounder - business strategy for vibecoders.
```

## Common Mistakes

- **Pitching instead of listening.** The number one mistake. The moment you say "So I built this app that...", the interview is over. They'll be polite, not honest.
- **Asking hypothetical questions.** "Would you pay $10/month for this?" always gets a yes. "How much do you currently spend on solving this?" gets the truth.
- **Interviewing friends and family.** They love you. They'll lie to protect your feelings. Interview strangers or acquaintances who have no reason to be nice.
- **Not recording.** You will forget 80% of what was said by the next day. Record (with permission) or take detailed notes.
- **Stopping after 2-3 interviews.** Patterns don't emerge until interview 5-8. One interview is an anecdote. Eight interviews are data.

## Notes

- This skill takes 10-15 minutes to generate the script
- The actual interviews take 25-30 minutes each
- Recommend doing 8-12 interviews over 2-3 weeks
- If running as part of /discover-customers, carry the target audience and mini-ICP into the script for tailored questions
- The note-taking template feeds directly into the summarize-interview skill

**Framework attribution**: Interview methodology from Rob Fitzpatrick, "The Mom Test" (2013). JTBD interview structure from Clayton Christensen, "Competing Against Luck" (2016). See CONVENTIONS.md for full attribution table.

---

### Further Reading

- [How to Do Customer Interviews That Don't Suck](https://fantasticfounder.com) - Running customer interviews using The Mom Test for vibecoders who've never done research before

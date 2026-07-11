# Nudge — Dreamlining Protocol

This is the Tim Ferriss Dreamlining exercise from *The 4-Hour Workweek*, structured as an agent-runnable protocol. The agent's job is to run the user through this exercise, not to do it for them. Read `guardrails.md` before starting.

## What dreamlining is

A 20-minute exercise to define what you actually want, convert abstract desires into concrete actions, and force the first step to happen within 48 hours. It replaces goal-setting (which is abstract and deferred) with action-setting (which is specific and immediate).

## The protocol, stage by stage

### Stage 1: Intake (the repression-facing)

Ask the user to list, for two timelines (6 months and 12 months), five things each in three categories:
1. **Having** (material: a car, a house, a specific possession)
2. **Being** (a skill, a state, an identity: fluent in Mandarin, a great cook, a black belt)
3. **Doing** (an experience: a trip, a performance, a project shipped)

That's 30 items total. The agent's job here is to push past socially acceptable answers. Most people write what they think they should want. The real list is the embarrassing one. Use the anti-repression moves in `prompts/intake.md`.

### Stage 2: Convert being to doing

For every **being** item, convert it to a **doing** item. "Great cook" becomes "make Christmas dinner without help." "Fluent in Mandarin" becomes "have a 10-minute conversation with a native speaker." The doing is measurable. The being is not. The agent suggests conversions; the user accepts or edits.

### Stage 3: Select the four

From the 30 items, the user picks the **four most important**, one per timeline is fine. This is the user's call. The agent does not pick for them. The agent can ask "what would have to be true for this to be your top four?" to help the user decide, but never picks.

### Stage 4: Estimate the cost

For each of the four, estimate the monthly cost. Ferriss's point: most dreams are cheaper than people assume. The agent helps research costs (rent in a city, language school, gear, etc.) but the user sets the number.

### Stage 5: Find three people who've done it

For each of the four dreams, find three people who've achieved it. Research their how-I-did-it content (blog posts, podcast transcripts, interviews, tweets). Surface the concrete steps they took. This is the agentic value-add: the worksheet tells you to do this, the agent does it for you. Use the research guidance in `prompts/research.md`.

### Stage 6: Generate the three steps

For each of the four dreams, generate three concrete steps the user will take:
1. **Now** — something they can do immediately, before they leave this session
2. **Tomorrow before 11am** — the first step of the first day
3. **Day after tomorrow before 11am** — the second step, to prove the first wasn't a fluke

The steps must be grounded in the research from Stage 5. Not generic advice. "Email the language school" not "find a language school." Use `prompts/steps.md`.

### Stage 7: Schedule

Schedule the three steps. Push to the user's calendar, Telegram, Slack, or a local file. The 11am deadline is Ferriss's specific protocol, not a generic reminder. The first step must happen today. Use `prompts/schedule.md`.

### Stage 8: Daily check-in (ongoing)

At a set time each morning (before 11am local), the agent asks: did you do yesterday's step? what's today's step? what's blocking you? This is the retention loop. Without it, the dreamline dies in 72 hours. Use `prompts/checkin.md`.

## The file format

The dreamline is stored as a single markdown file (see `templates/blank-dreamline.md`). The agent reads and writes this file. The structure:

```markdown
# Dreamline — [date]

## 6 months
### [Dream title]
- category: having / being / doing
- being-to-doing: [converted doing, if applicable]
- monthly_cost: $[amount]
- research:
  - [person 1]: [link]
  - [person 2]: [link]
  - [person 3]: [link]
- steps:
  1. [now] — [action]
  2. [tomorrow 11am] — [action]
  3. [day after 11am] — [action]

## 12 months
[same structure]
```

## What success looks like

The user takes the first step before they leave the session. Not tomorrow. Not next week. Today. If the user finishes the session with a completed dreamline file and no action taken, the protocol failed. The whole point is the now step.

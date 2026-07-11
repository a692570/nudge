# nudge

An installable dreamlining protocol for agentic coding assistants (Codex, Claude Code, Cursor, Hermes, any agent that reads markdown).

Based on Tim Ferriss's Dreamlining exercise from *The 4-Hour Workweek*. The agent runs you through the full Ferriss protocol: name what you actually want, convert being to doing, find people who've done it, generate the three steps, schedule the now/tomorrow/day-after actions.

**Nudge assists. It does not replace.** The agent will not name your dreams for you, write your steps without your input, or take the actions in your place. The repression-facing is the exercise. Skip it and the whole thing is worthless.

## Install

Drop the `nudge/` directory into your agent's skills folder. The agent picks up `protocol.md` as the runnable protocol, `prompts/` for the interview stages, `guardrails.md` for the stop points.

## What's inside

- `protocol.md` — the dreamlining exercise, structured as an agent-runnable protocol
- `prompts/` — stage-by-stage interview prompts (intake, being-to-doing, research, step generation, scheduling, daily check-in)
- `templates/` — blank dreamline templates the agent fills with you
- `examples/` — one worked example so the agent understands the output shape
- `guardrails.md` — the assist-don't-replace boundary, the most important file

## License

MIT

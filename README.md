# nudge

Most people know what they want. They just haven't taken the first step.

Nudge is a small set of prompts and templates you install into your AI coding assistant (Codex, Claude Code, Cursor, Hermes, anything that reads markdown). Your agent runs you through a short exercise that turns the things you keep saying you want into actions you take this week.

Not next month. Not Monday. Today, before you close the chat.

## The problem it solves

You have a list of things you want. Learn a language. Live in another country. Write a book. Start a project. The list sits there. You'll get to it. You never get to it.

The gap between wanting and doing is not a motivation problem. It's a structure problem. Most goals are too vague to act on, too far away to start, and too unscheduled to survive the first busy week.

Nudge fixes the structure. It runs you through a short exercise that:

1. **Forces you to name what you actually want**, not what sounds good to say out loud. The embarrassing version. The Ferrari. The move to Tokyo. The thing you'd be shy to tell your parents.
2. **Converts states into actions.** "Be a great cook" is a state with no endpoint. "Cook Christmas dinner for 8 people without help" is an action you can take.
3. **Finds three people who've done each thing** and shows you the concrete steps they took. You're not guessing at the path. You're following a path that worked.
4. **Generates three steps you take now, tomorrow before 11am, and the day after before 11am.** Specific, grounded in the research, doable without anyone's permission.
5. **Checks in with you each morning** until the chain holds. Three days. Three steps. By day three, you've moved.

## Where it comes from

The exercise was originally designed by Tim Ferriss in *The 4-Hour Workweek*. He called it "dreamlining." The name never stuck. It sounds like a vacation brochure. The exercise itself is sharper than the name suggests: a structured way to stop deferring the things you say you want.

Nudge takes that exercise and packages it for the tool you already use. You don't have to read the book. Your agent runs you through it.

## What it is not

Nudge does not name your dreams for you. It does not write your steps without your input. It does not take the actions in your place. The whole point is the part where you face what you want and commit to a first step. If the agent did that work, the exercise would be worthless. Nudge is a coach that refuses to do the reps for you.

## Install

Drop the `nudge/` directory into your agent's skills folder. The agent reads `protocol.md` as the runnable exercise, `prompts/` for each stage, `guardrails.md` for the stop points.

If your agent doesn't have a skills folder, just point it at the repo and ask it to run you through the protocol in `protocol.md`.

## What's inside

- `protocol.md` — the full exercise, stage by stage
- `guardrails.md` — where the agent stops (the assist-don't-replace boundary)
- `prompts/` — the prompts for each stage (intake, being-to-doing, research, steps, schedule, daily check-in)
- `templates/` — the blank file the agent fills with you
- `examples/` — one worked example so you can see what the output looks like

## License

MIT

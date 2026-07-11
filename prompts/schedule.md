# Stage 7 prompt — Schedule

Schedule the three steps. The first step must happen today, before the session ends. The tomorrow and day-after steps must be set for before 11am local time.

## Delivery options

The agent should detect or ask which channels the user has available:
- **Calendar** (Google Calendar, Apple Calendar, Outlook) — create events with 11am start times and the step as the title
- **Telegram** — send a message to the user at 10:30am local time with the day's step
- **Slack** — same as Telegram, to a DM or a designated channel
- **Local file** — write to a `nudge-reminders.md` file the user can check, if no messaging channel is available
- **Plain text** — if no integrations are configured, output the schedule as text and tell the user to set the reminders manually

## The now step

The now step is not scheduled. It is taken before the session ends. The agent's job is to get the user to do it before they close the chat. If the user tries to defer, see `guardrails.md` — name the deferral, push for the smallest possible version of the step.

If the step is "email the Berlitz school," the agent stays with the user until the email is drafted and sent. If the step is "book a trial lesson," the agent waits while the user books it. The session doesn't end until the now step is done.

## The 11am reminder

For the tomorrow and day-after steps, schedule a reminder for 10:30am local time. The reminder is not just a ping. It includes:
- The step (one sentence)
- The person whose path this step came from (the research link)
- A line: "this is your 11am step. take it before the day's friction accumulates."

## Refusals to schedule

If the user refuses to schedule the tomorrow and day-after steps, the agent notes the refusal in the dreamline file and ends the session. The now step still has to happen. Refusing to schedule is a softer version of refusing to act. The agent names it: "you've taken the first step. scheduling the next two is what makes it a chain instead of a single action. let's set them."

## Pacing

2-3 minutes. Don't over-engineer. The schedule is a means to the action, not a productivity system.

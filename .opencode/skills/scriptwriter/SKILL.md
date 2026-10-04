---
name: scriptwriter
description: Write Taglish content scripts from an approved content strategy. Use this skill when a user or content orchestrator hands off a strategy report or asks to turn an approved content format into a script. Read the report from the conversation or `docs/strategy/<slug>.md`; do not add facts that the report does not support.
---

# Scriptwriter

Convert an approved content strategy into a clear, usable Taglish script while preserving its evidence, intent, and constraints.

## Find and validate the handoff

- Use the strategy report supplied in the conversation or read `docs/strategy/<slug>.md` when the orchestrator identifies the slug/location. The preceding skill is named `content-strategy` (the corresponding agent may be named `content-strategist`).
- Find the topic slug, goal, audience, approved content format, required points, sources, and constraints before drafting.
- The format must be approved. If the report says approval is pending or does not establish an approved format, ask the orchestrator/user for approval rather than choosing one yourself.
- If the report is missing, vague, contradictory, or lacks information essential to produce the requested script, explain what is unclear and ask the orchestrator for a corrected/complete handoff. Do not compensate by inventing content.

## Write the script

- Follow the approved format and the report's audience, goal, key message, verified facts, and constraints.
- Write naturally in Taglish: use Filipino and English fluidly for the intended audience. Preserve proper nouns and technical terms where needed.
- You may make the wording engaging and easy to speak, but every factual claim, promise, statistic, and substantive point must be supported by the strategy report. Do not add facts from memory or outside research.
- Make format-specific structure clear when helpful (for example, scene/visual, spoken line, on-screen text, and timing for a video). Do not impose a length or platform that the report does not specify; ask if it materially affects the script.
- Keep source/verification context available in a short note or source list when the strategy provides it; do not turn citations into spoken dialogue unless requested.

## Output and saving

- Present the script in Taglish in the response.
- Save the script by default as Markdown at `docs/scripts/<slug>.md`, using the strategy's slug. Create the parent directory if needed. If no slug is supplied, derive a concise lowercase hyphenated slug from the topic and use it consistently.
- Do not overwrite an existing script without asking. If file writing is unavailable, provide the full script in the response and state that it was not saved.
- Use a useful title and headings appropriate to the approved format. Keep any factual note or source list separate from the spoken script.

## Boundaries

- Your role is to write the script from the strategy, not to redo the strategy, change its approved format, or write social posts.
- Do not introduce facts, claims, examples, calls to action, or promises absent from the report. A call to action is allowed only when consistent with the stated goal and report.
- When a limitation blocks a faithful script, notify the orchestrator instead of guessing.

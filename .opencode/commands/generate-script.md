---
description: Generate and save a Taglish script from an approved content strategy
agent: content-orchestrator
---

Generate a script using the conversation and any supplied context: $ARGUMENTS

1. Find the content strategy report in the current conversation or, when its slug is known, read `docs/strategy/<slug>.md`.
2. Check that the report includes an approved content format, topic slug, goal, audience, required points, and constraints. A recommendation marked pending approval is not approval. If the report is missing, unclear, or the format is not approved, stop and ask the user or orchestrator for the missing handoff; do not guess or draft around it.
3. Delegate the script-writing work to the `scriptwriter` agent and have it follow the `scriptwriter` skill. Pass the full strategy report and any user-provided direction, while treating the report as the source of truth for claims and facts.
4. Have the agent write a natural Taglish script that follows the approved format. Do not add unsupported claims or change the approved format.
5. Save the Markdown script to `docs/scripts/<slug>.md`, reusing the report's slug. Create the parent directory if needed. If that file already exists, do not overwrite it without asking first.
6. Confirm the saved path and briefly summarize the result. If a blocker prevents saving, provide the script in the response if it can be produced faithfully and clearly explain that it was not saved.

Example: `/generate-script Create a script from the approved grocery-planning strategy above.`

Done when the script is faithfully based on an approved strategy and saved at `docs/scripts/<slug>.md`, or when a blocking issue is reported instead of guessing.

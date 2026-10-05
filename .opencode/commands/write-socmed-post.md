---
description: Create and save a Taglish social post from a completed script
agent: content-orchestrator
---

Create a promotional social media post from the completed script in the conversation or designated file: $ARGUMENTS

1. Identify the topic slug from the conversation or user-provided location. If a completed script is included in the conversation, use that; otherwise read `docs/scripts/<slug>.md`.
2. If the script cannot be found, is unreadable, or does not contain enough information to identify the content being promoted, stop and request the completed script. Do not write a post from a topic alone.
3. Delegate the post-writing work to the `social-media-writer` agent and have it follow the `social-media-writer` skill. Pass the complete script, topic slug, and any requested platform or post constraints.
4. Have the agent write an engaging, natural Taglish post based only on the script. Do not add unsupported claims, promises, details, or urgency. If no platform is specified, keep the post platform-neutral.
5. Save the Markdown post to `docs/post/<slug>.md`, reusing the script's slug. Create the parent directory if needed. If that file already exists, do not overwrite it without asking first.
6. Confirm the saved path and briefly summarize the result. If a blocker prevents saving, clearly report it rather than claiming the post was saved.

Example: `/write-socmed-post Create a post from the completed script at docs/scripts/meal-prep.md for Instagram.`

Done when the post is faithfully based on the completed script and saved at `docs/post/<slug>.md`, or when a blocking issue is reported instead of inventing source content.

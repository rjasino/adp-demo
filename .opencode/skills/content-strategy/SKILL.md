---
name: content-strategy
description: Develop evidence-backed content strategies from briefs handed off by a content orchestrator. Use this skill whenever a user or orchestrator asks what content to create, needs an audience or goal clarified, wants a recommendation for a content format, or requests strategy before scripting. Research factual topics, recommend a format, and do not write the script.
---

# Content Strategy

Turn an orchestrator's topic brief into a practical, researched strategy that a scriptwriter can use after the user approves a content format.

## Inputs and clarification

- Use the current conversation or explicit handoff from the `content-orchestrator` as the brief. Look for the topic, campaign goal, target audience, geography, platform, constraints, and any approved format.
- Do not silently fill gaps with assumptions. If the topic itself is unclear, ask a focused clarifying question before researching. If other missing details would materially change the recommendation, ask for them; otherwise identify them as unknown and make a clearly qualified recommendation.
- Separate information supplied by the user from findings verified through research. Never present an inference as a confirmed fact.

## Workflow

1. Create a short, stable slug from the topic: lowercase words separated by hyphens; omit punctuation and keep it concise. Reuse a slug already supplied by the orchestrator or established in the conversation.
2. Research claims and context that matter to the strategy. Prefer primary or authoritative sources, check dates and geography, and cite links next to relevant findings. Use available browsing/research tools. If research is unavailable or a claim cannot be verified, say so rather than implying verification.
3. Identify the content goal and audience from the brief. When either is unknown, state that explicitly instead of inventing one.
4. Recommend a content format suited to the goal, audience, platform, and evidence. Explain briefly why it fits and note reasonable alternatives only when useful. A recommendation is not user approval: if no format is approved, leave the scriptwriter a clear approval dependency.
5. Present the strategy report in the conversation by default. Save it only when the user asks to save it or otherwise clearly expresses intent to keep the document. When saving, write Markdown to `docs/strategy/<slug>.md` (create the parent directory if needed). Do not overwrite an existing report without asking first.

## Report structure

Use this Markdown structure, adapting sections only when information is genuinely unavailable:

```markdown
# Content Strategy: <Topic>

## Brief
- Topic:
- Goal:
- Target audience:
- Geography/platform:
- Constraints:

## Audience and goal
<What is known, what remains unknown, and the intended audience need or action.>

## Research and verified context
<Relevant findings, with source links and dates where available. Distinguish verified facts from brief-provided context.>

## Recommended content format
<One primary recommendation, why it fits, and whether it is awaiting user approval.>

## Strategic direction
<Key message, angle, and useful content beats or proof points. Do not write dialogue or a finished script.>

## Handoff to scriptwriter
- Topic slug:
- Approved content format: <approved format, or "pending user approval">
- Goal and audience:
- Required points / verified facts:
- Sources:
- Constraints and open questions:
```

## Boundaries

- Provide research, audience/goal analysis, format advice, and strategic direction only. Do not write a script, caption, or finished post.
- Do not invent facts, sources, audience attributes, campaign results, or user approval.
- Ask for clarification when ambiguity prevents a responsible strategy; otherwise make uncertainty visible in the report.

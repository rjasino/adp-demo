## AI Agent Tool

- Choose the Model
  - Claude (Reasoning)
    - Haiku 4.5
    - Sonnet 5
    - Opus 5.5
    - Fable 5.1
  - GPT (General Purpose)
    - GPT 5 Series
    - GPT 6 Luna
    - GPT 6 Sol
    - GPT 6 Astra
  - Gemini (Multimodality)
  - Deepseek (Reasoning)
  - Kimi (Coding)
  - MiniMax
  - Qwen
  - GLM (Coding)
  - Grok
  - Jev
- Choose the Harness
  - Claude App (Cowork, Chat and Code)
  - ChatGPT Codex
  - Antigravity
  - OpenCode
  - Cursor
  - Github Copilot
  - Pi

Social Media Content Generation Workflow

- Agents
  - content-orchestrator - primary
  - content-strategist - subagent
  - scriptwriter - subagent
  - social-media-writer - subagent
- Skills
  - content-strategy
  - scriptwriting
  - social-media-writing
- Commands
  - generate-script
  - write-socmed-post

  when we interact with our agent, we describe what we want.
  /generate-script
  /write-socmed-post

## Pointer

- Agents - Persona (Role and Identity)
- Skills - Capabilities (Repetitive and Specialized Tasks)
- Commands - Orchestration (Workflow)

- Timestamp
- Intro - 00:00
- Building Blocks of Agentic Workflow - 00:35
- What are Agents (Custom Agents and Subagents) - 01:14
- What are Skills - 03:54
- What are Commands - 05:23
- Example Workflow to produce - 06:55
- Start of Implementation - 19:48
- OpenCode Harness - 21:46
- Writing your first custom agent - 27:00
- Testing our workflow - 52:10

https://www.youtube.com/watch?v=pzKPcN9yMis

teach about node and git

- node is a javascript runtime that allows you to run javascript code outside of a browser. it is being use in web application development for both fronend and backend.
- git is a version control system that allows you to track changes in your code and collaborate with others. it is widely used in software development to manage source code and keep track of different versions of a project.
- download and install node and git from their official websites.

---

## Tools needed

- Git
  - version control -> github (remote repository)
  - it use to track changes on files
- Node
  - javascript runtime use in web app development
  - it will be use to execute packages and script
  - other install python
  - powershell, cmd
  - bash, zsh
- VS Code
  - the code? text editor of choice
  - a lot of quality of life to format and enhance our experience
- OpenCode
  - you can use either TUI or Desktop App
  - we defaulted to Desktop App

---

skills.sh -> user generated skills

- skill-creator
- command-creator
- install via npx

what skills have

- input
  - conversation
  - file
    - text
    - image
    - video
  - handoff
- process
- guardrails
- output
  - format
  - location
  - response type
  - tone

what commands have

- usage (example)
- steps
- definition of done

wire up the skill with the agent
test the workflow
compare the output from the previous generation
use the same prompt

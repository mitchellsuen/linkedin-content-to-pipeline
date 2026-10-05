# LinkedIn Content to Pipeline

**Turn what you know into content, identify the right people engaging with it, and start useful sales conversations.**

This is the shareable template behind my LinkedIn funnel. Make your own copy, add your experience and offer, and build the system around the people you want to help.

**[Use this template →](https://github.com/new?template_name=linkedin-content-to-pipeline&template_owner=mitchellsuen)** · [Browse all skills](skills/README.md) · [Download ZIP](https://github.com/mitchellsuen/linkedin-content-to-pipeline/archive/refs/heads/main.zip)

## What you get

| Included | What it helps you do |
|---|---|
| [23 core content and branding skills](skills/README.md#the-23-core-skills) | Research, write, repurpose and design content in your own voice |
| [6 additional video skills](skills/README.md#additional-video-skills) | Keep the full content-vault skill coverage, including Shorts and Manim |
| [Your personal-brand second brain](context/index.md) | Give your agent your positioning, audience, voice, stories and proof |
| [Notion setup](guides/notion.md) | Organize your pillars, topics, hooks and content board |
| [ICP qualification templates](guides/qualification.md) | Score company fit and person fit, with evidence and reasons |
| [DM conversion framework](guides/dm-conversion.md) | Deliver the resource, understand the problem and agree on a next step |
| [High-resolution flowchart](assets/linkedin-funnel.png) · [Editable file](assets/linkedin-funnel.excalidraw) | See how the whole funnel connects |

All skills are in the visible **[`skills/`](skills/)** folder. There are **29 in total**: 23 core skills and 6 additional video skills. The [catalog](skills/README.md) shows where every original content-vault skill lives.

## Start here

1. Click **[Use this template](https://github.com/new?template_name=linkedin-content-to-pipeline&template_owner=mitchellsuen)** and create your own repository. Choose **Private** if you will add personal or customer information.
2. Clone your copy and open the whole folder in Codex, Claude Code or your preferred coding agent. You can also download the ZIP to work locally.
3. Paste this prompt:

```text
Read AGENTS.md and README.md. Help me make LinkedIn Content to Pipeline my own.
Use setup-workspace, capture-context and voice-calibration to build my
context from the material I provide. Start with my audience, offer,
experience and writing samples. Ask for the few missing details that
matter, keep unknown claims empty, and draft my first useful LinkedIn
post in chat using linkedin-copywriter.
```

Bring your offer, a short interview or notes, and 5–10 representative writing samples if you have them. The [context interview](context/templates/context-interview.md) gives you a starting point. **You can create your first post without Notion or any other tool.**

The repository includes skill-discovery links for Codex and Claude Code. If your agent does not discover them, point it to `skills/README.md` and the relevant `SKILL.md` file.

## The three parts

### 1. Create content that attracts the right people

Fill your [second brain](context/index.md), define your audience and calibrate your voice. Use `linkedin-copywriter` for one post, `week-posts` for a weekly plan and `lead-magnet-creator` for a resource your readers can use. Set up [Notion](guides/notion.md) when you want a content board.

### 2. Find the people who fit

Export the people engaging with your posts from the LinkedIn tool you already use into a table. Then follow the [qualification guide](guides/qualification.md): the [qualification prompt](templates/qualification-prompt.md), [rubric](templates/icp-rubric.md) and [output schema](templates/qualification-output.schema.json) assess company and person fit separately.

When you have an engager list, paste this into your agent:

```text
Read guides/qualification.md. Use my ICP and offer to prepare the
qualification rubric in company/private/. Then inspect the columns in
[MY ENGAGER EXPORT], map them to the prompt's evidence fields and score
one row with me before running the rest.
```

Collection and AI scoring may each have usage costs in the tools you choose. Calibrate on a small reviewed set before scoring a full list.

### 3. Turn relevant interest into conversations

Use the [DM framework](guides/dm-conversion.md) to deliver what someone requested, learn what they need and offer a useful next step. Review the qualified cohort yourself before starting any outreach, whether you message by hand or through an outreach tool.

Track qualified conversations, opportunities and signups alongside reach. That is how you see whether your content is helping the business.

## Make it yours

```text
skills/       Content, branding and media instructions
context/      Your blank personal-brand and second-brain scaffold
guides/       Notion, qualification and DM setup
templates/    Editable ICP rubric, qualification prompt and output schema
examples/     Synthetic qualification decisions to calibrate against
company/      Example buyer rubrics; keep your own in company/private/
assets/       High-resolution funnel and editable Excalidraw
```

The scaffold starts blank. Use your own biography, voice and proof when filling it.

The funnel artwork illustrates my system. Use it as a reference for your setup. Your results will depend on your audience, offer, content and follow-through.

Built by [Mitchell Suen](https://github.com/mitchellsuen): master AI agents and build automation workflows that fill their pipeline. [Sources and scope](guides/sources.md) · [License](LICENSE)

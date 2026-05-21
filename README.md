# instagram-carousel-agent
A Skill with a multi-agent system for generating end-to-end Instagram carousel content — hooks, body slides, visuals, CTA, captions, and hashtags.

# 📱 Instagram Carousel Agent

A Claude Skill that runs a multi-agent pipeline to produce complete Instagram 
carousel content from a single brief — no prompt engineering required.

## What it does

Give it a topic and audience. It activates 6 specialized sub-agents in sequence:

- 🪝 **Hook Specialist** — writes 3 scroll-stopping Slide 1 hooks
- ✍️ **Content Writer** — produces punchy body slides (one idea per slide)
- 🎨 **Visual Director** — defines color palette, fonts, and layout spec
- 📣 **CTA Specialist** — closes with a conversion-focused final slide
- 🔍 **SEO & Hashtag Strategist** — writes the caption + 25-tag hashtag stack
- ♻️ **Content Repurposing Agent** — adapts the carousel into Reels, threads, LinkedIn & email

## How to use

1. Download the `.zip` from [Releases](#)
2. In Claude.ai → Settings → Features → Skills → `+` → Upload ZIP
3. Start a chat and say: *"Create a carousel about [your topic]"*

## Built with

- [Claude Skills](https://support.claude.com) — Anthropic's reusable instruction format
- Compatible with Claude.ai, Claude Code, and the Claude API

## Contributing

Contributions welcome! Open an issue to suggest new agents or improvements.

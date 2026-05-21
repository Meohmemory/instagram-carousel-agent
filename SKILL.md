---
name: instagram-carousel-agent
description: Use this skill when the user wants to create Instagram carousel content. Triggers include: requests to write a carousel, create Instagram slides, plan carousel content, write hooks for Instagram, or produce multi-slide Instagram posts. This skill activates a full multi-agent system including a Hook Specialist, Content Writer, Visual Director, CTA Specialist, SEO & Hashtag Strategist, and Content Repurposing Agent. Use when user mentions "carousel", "Instagram slides", "swipe post", "hook for Instagram", or "carousel content".
---

# 📱 Instagram Carousel Agent System

A complete multi-agent framework for producing end-to-end Instagram carousel content.

## Workflow Pipeline

When asked to create a carousel, follow this agent sequence:

```
Brief Input → Hook Specialist → Content Writer → Visual Director → CTA Specialist → SEO & Hashtag Strategist → (optional) Repurposing Agent → Final Carousel
```

---

## 🎯 Step 1 — Parse the Brief (Orchestrator)

Before delegating, extract:
- **Topic**: What is the carousel about?
- **Target Audience**: Who is this for?
- **Goal**: Follow / Save / DM / Link click?
- **Tone**: Educational / Storytelling / Listicle?
- **Slide count**: Default to 7 slides if not specified

---

## 🪝 Step 2 — Hook Specialist (Slide 1)

Write **3 hook variations** for the first slide. Each hook must:
- Lead with a bold, curiosity-driven statement
- Use power words: "Stop", "Secret", "Why most people fail at…", or numbers
- Be under 10 words on the headline
- Create a pattern interrupt that stops the scroll

**Output format:**
```json
{
  "hooks": [
    { "headline": "...", "subheadline": "...", "hook_type": "curiosity/number/challenge" }
  ]
}
```

Present the 3 options and ask the user to pick one before continuing.

---

## ✍️ Step 3 — Content Writer (Slides 2 to N-1)

Write body slides using the selected hook. Rules:
- ONE main idea per slide
- Headline: max 6 words
- Body copy: max 30 words
- End each slide with a micro-cliffhanger to drive the next swipe
- Maintain consistent tone throughout

**Output format:**
```json
{
  "slides": [
    { "slide_number": 2, "headline": "...", "body": "...", "visual_hint": "..." }
  ]
}
```

---

## 🎨 Step 4 — Visual Director

Produce a visual specification for the carousel:
- **Color palette**: background, primary text, accent (3 colors)
- **Font pairing**: headline font + body font
- **Layout**: define template for hook slide, body slides, and CTA slide
- **Style notes**: icon style, illustration direction, mood

---

## 📣 Step 5 — CTA Specialist (Final Slide)

Write the closing CTA slide aligned with the content goal:
- Headline: clear action statement (max 8 words)
- Sub-copy: reinforce the value (max 20 words)
- Primary CTA: one action — Save this / DM me / Follow / Link in bio
- Optional: social proof or urgency line

---

## 🔍 Step 6 — SEO & Hashtag Strategist

Write the Instagram caption and hashtag set:

**Caption rules:**
- First line must hook the algorithm (under 125 characters)
- Include a call-to-action in the caption body

**Hashtag tiers (25 total):**
- Niche tags (under 100k posts): 10 tags
- Mid-range tags (100k–1M posts): 10 tags
- Broad tags (1M+ posts): 5 tags

---

## ♻️ Step 7 — Content Repurposing Agent (Optional)

If the user asks to repurpose, adapt the carousel into:
1. **Instagram Reels script** — hook + 3 talking points + CTA (30–60 seconds)
2. **Twitter/X thread** — hook tweet + 5–7 follow-up tweets
3. **LinkedIn post** — professional angle, 150–200 words
4. **Email newsletter snippet** — subject line + 100-word body

---

## 📦 Final Deliverable

Present the complete carousel package:

```
✅ Slide 1: [Selected Hook]
✅ Slides 2–N-1: [Body content]
✅ Slide N: [CTA]
🎨 Visual Spec: [Colors + Fonts + Layout]
🔍 Caption + 25 Hashtags
♻️ Repurposed content (if requested)
```

---

## Agent Quick Reference

| Agent | Slide | Focus |
|-------|-------|-------|
| 🪝 Hook Specialist | Slide 1 | Scroll-stopping first impression |
| ✍️ Content Writer | Slides 2–N-1 | One insight per slide, swipe momentum |
| 🎨 Visual Director | All slides | Colors, fonts, layouts |
| 📣 CTA Specialist | Last slide | Conversion action |
| 🔍 SEO Strategist | Caption | Discoverability & reach |
| ♻️ Repurposing Agent | Post-production | Cross-platform content |

---
name: brand-story
description: Creates the emotional foundation of a brand before any visual work begins. Maps emotional territory, finds the human meaning, and crafts a 6-paragraph emotive narrative that prevents generic AI-slop design. Use before briefing a designer, writing copy, or starting a brand process.
version: 1.0.0
tools:
  - Read
  - Bash
  - Write
  - WebFetch
  - mcp__perplexity__perplexity_ask
license: MIT
---

# Brand Story

Write the soul of a brand before anyone touches a logo.

This skill produces an emotive narrative — 6 paragraphs that capture the human meaning behind a product. It's the emotional context that every design decision should be testable against. Without it, you get technically correct but soulless design.

## Command

```
/brand-story "Project Name"
/brand-story "Project Name" projecturl.com
```

---

## Why this exists

LLMs default to generic. Ask Claude to design a brand and you get rounded corners, purple-to-blue gradients, and "clean and modern." The antidote isn't more design instructions — it's deep emotional context established before any visual work begins.

This narrative becomes the standard every subsequent choice is tested against:
> "Does this font express what we said about quiet confidence? No? Then why is it here?"

---

## Pipeline

### Step 0 — Understand the project

If a URL or codebase is available, read it. Look for:
- What the product actually does (not what it says it does)
- Who it's for — infer from tone, technical level, examples
- What problem it solves and for whom
- Any existing language that feels alive or dead

If nothing is available, ask one question: "What does this product do and who is it for?"

---

### Step 1 — Map the emotional territory

Work through four lenses. Don't present these to the user — use them internally to build understanding.

**Emotional transformation**
What state does the user arrive in? What state do they leave in?
Format: From [negative] → To [positive]
Example: From anxiety about complexity → To quiet confidence it's handled

**Brand archetype**
Pick the primary archetype and one complementary trait:

| Archetype | Core desire | Emotional appeal |
|-----------|-------------|------------------|
| The Hero | Mastery, courage | Empowerment, achievement |
| The Sage | Understanding, truth | Wisdom, clarity |
| The Explorer | Freedom, discovery | Adventure, autonomy |
| The Creator | Innovation, expression | Imagination, originality |
| The Caregiver | Service, compassion | Nurturing, protection |
| The Ruler | Control, order | Authority, stability |
| The Magician | Transformation, vision | Wonder, possibility |
| The Rebel | Liberation, disruption | Revolution, independence |
| The Everyman | Belonging, authenticity | Relatability, honesty |

**Sensory vocabulary**
Build 8–10 words or phrases across:
- Visual (light/dark, sharp/soft, sparse/dense)
- Tactile (smooth, heavy, solid, fluid)
- Spatial (expansive, layered, enclosed, open)
- Movement (flowing, settling, ascending, pulsing)

**Emotional jobs**
- Functional: what task does it perform?
- Emotional: how does it make them feel?
- Social: how does it affect how they see themselves?

---

### Step 2 — Write the narrative

Six paragraphs. Write as if capturing something that deeply matters. This is not marketing copy.

**Paragraph 1 — The Human Moment**
Open with a concrete scene. Show the friction, the frustration, or the desire. Don't say "users need X" — show the moment before they had this.

**Paragraph 2 — The Deeper Truth**
What does that moment reveal? Connect to something universal. Name the tension or paradox at the heart of it.

**Paragraph 3 — The Transformation**
What becomes possible when this exists? Write the after-state in sensory, emotional language. Focus on the human change, not the technical feature.

**Paragraph 4 — The Ethos**
What does this product believe? What is it saying no to? What quality of experience is it committed to?

**Paragraph 5 — The Personality**
How does it move through the world? What energy does it carry? Not its features — its character.

**Paragraph 6 — The North Star**
The decision filter. One guiding question that, when design choices are hard, points the way.

---

### Step 3 — Validate before presenting

Before showing the narrative, check:

- **Specificity** — Could this only be written about this product, or would it fit any similar one?
- **Emotion** — Does reading it produce a feeling?
- **Guidance** — Could someone make a design decision based on this?
- **Humanity** — Is there a human at the centre, not just a product?
- **Conviction** — Does it take a clear stance?

If any answer is no, revise.

---

### Step 4 — Present and confirm

Show the narrative. Ask: "Does this capture what you're building? Anything that doesn't ring true?"

Revise based on feedback. One round.

---

### Step 5 — Write to file

Save as `[project-name]-brand-story.md` in the current directory.

Output format:

```markdown
# [Brand Name] — Brand Story

## The Human Moment
[Paragraph 1]

## The Deeper Truth
[Paragraph 2]

## The Transformation
[Paragraph 3]

## The Ethos
[Paragraph 4]

## The Personality
[Paragraph 5]

## The North Star
[Paragraph 6]

---
*Generated with /brand-story — https://github.com/b1rdmania/brand-story*
```

---

## Voice rules

- Concrete and specific, never generic
- Sensory language — sight, touch, space, movement
- Short paragraphs. No hedging.
- No buzzwords. No "revolutionary", "seamless", "powerful"
- Present tense
- If it could describe any brand, cut it and start again

---

## What this is not

- Not marketing copy
- Not a product description
- Not a list of features
- Not a mission statement
- Not a tagline

It is the emotional context that makes all those things better.

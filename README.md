# brand-story

Write the emotional foundation of a brand before any visual work begins.

---

## The problem with AI design

Ask an LLM to design a brand and you get rounded corners, Inter or Roboto, a purple-to-blue gradient, and something described as "clean and modern." Every time. Not because the model is bad — because it defaults to statistical mean. It has seen ten thousand SaaS landing pages and it averages them.

The fix is not better design prompts. The fix is richer context established *before* you ask for anything visual.

Specifically: metaphor.

When you tell an LLM that a brand should feel like "the quiet hum of a power grid — invisible, reliable, present only when it fails," you have given it something to work *from*. A sensory anchor. An emotional territory. A standard every subsequent choice can be tested against. That prompt produces different typography, different colour instincts, different spatial decisions than "make it feel professional and modern."

`/brand-story` creates that context. It maps the emotional territory of a product using brand archetypes, Plutchik's emotional wheel, and a Jobs-to-be-Done emotional frame — then reduces it to a six-paragraph narrative built on concrete metaphor. The narrative becomes the brief. Everything after it has somewhere to go.

---

## What it produces

A six-part emotive narrative saved to `[project]-brand-story.md`:

| Section | What it captures |
|---|---|
| The Human Moment | The scene before your product exists — concrete, specific, felt |
| The Deeper Truth | What that moment reveals about why this matters |
| The Transformation | What becomes possible — in human, not technical terms |
| The Ethos | What this product believes and what it refuses to be |
| The Personality | How it moves through the world |
| The North Star | The one question that settles hard design decisions |

---

## Install

```bash
git clone https://github.com/b1rdmania/brand-story ~/.claude/skills/brand-story
```

Requires [Claude Code](https://claude.ai/code).

## Usage

```
/brand-story "Project Name"
/brand-story "Project Name" projecturl.com
```

Provide a URL and the skill reads the product before writing. No URL and it asks one question: what does this do and who is it for?

---

## Example output (Sorted.fund)

> **The Human Moment**
> Every game developer knows the moment: you've built something delightful, but then players need to make a transaction. Suddenly they're navigating wallet prompts, approving tokens, wondering why they need gas on a chain they've never heard of. The game disappears. The blockchain becomes foreground. Magic turns into homework.

> **The North Star**
> When unsure about a design decision: "Does this make our infrastructure more visible or less visible?" If we're showing off how clever we are, we're wrong. If we're disappearing so the game can shine, we're getting there.

That's the kind of brief an LLM can actually use. Not "make it feel trustworthy." Make it feel like the quiet confidence of a system that never needs to announce itself.

---

## What happens next

This narrative is the input to everything else — copy, visual direction, logo brief, design system. Paste it as context before any design conversation and watch the output change.

For the full brand process (visual direction, mark development, design system), see [claude-brand-skills](https://github.com/b1rdmania/claude-brand-skills).

## License

MIT

# Stop the Slop

A Claude Code skill to remove AI writing patterns entirely.

## Problem

Balaji Srinivasan [nailed it](https://x.com/balajis/status/1947947338007560569):

> "0% AI is slow. But 100% AI is slop. So the optimal amount of AI is actually between 0-100%... It's the Laffer Curve, but for AI."

As more people use AI to write, the output sounds the same. Predictable structures and hollow transitions. You spot it in the first sentence.

Use AI to write better, then strip the AI out of the prose.

## Why We Built This

We're [Flywheel](https://flywheelos.com/). We help leading companies, including Fortune 500s, with their content strategy.

Part of that process has been stripping out telltale signs of AI writing. After months of doing this manually, we codified the patterns into a skill.

## What It Catches

**10 patterns that standard grammar tools miss:**

1. **False Agency** - "The data tells us" (data doesn't tell, people read it)
2. **Narrator Voice** - floating above the scene instead of putting the reader in it
3. **Wh- Openers** - "What makes this hard is..." (just say what's hard)
4. **Vague Declaratives** - "The implications are significant" (name them)
5. **Negative Runway** - "Not X. Not Y. It's Z." (just say Z)
6. **Three-Item Lists** - AI loves triplets. Humans use two.
7. **Question Endings** - "What would you do?" (LinkedIn CTA energy)
8. **Over-Explanation** - defining terms readers already know
9. **Adverb Infestation** - genuinely, fundamentally, truly, inevitably
10. **Passive Hiding** - "Mistakes were made" (by whom?)

Plus: banned phrases, structure checks, and a specificity gate.

## Installation

```bash
# Clone the repo
git clone https://github.com/khwong72/stop-the-slop.git

# Symlink to your Claude Code skills directory
ln -s $(pwd)/stop-the-slop/skill ~/.claude/skills/stop-the-slop
```

Or copy `skill/` to `~/.claude/skills/stop-the-slop/`.

## Usage

After drafting and editing your content:

```
/stop-the-slop
```

Run the audit. If anything fails, fix it and re-run.

## Workflow

```
Draft → Edit → /stop-the-slop → Publish
```

This is a **final audit**, not a drafting tool. Run it after your content is polished.

## Test

Read it aloud.

- Sounds like a peer explaining over coffee → **Pass**
- Sounds like a LinkedIn post → **Fix it**
- Sounds like a keynote → **Fix it**

## Files

```
skill/
├── SKILL.md          # Main skill (run with /stop-the-slop)
├── banned-phrases.md # Structures, transitions, dramatic language
├── patterns.md       # The 10 AI tells with examples
└── examples.md       # Before/after transformations
```

## Contributors

- [@khwong72](https://github.com/khwong72)
- [@aliguy](https://github.com/aliguy)
- [Claude](https://claude.ai) - AI pair programmer

## License

MIT

---

Share this with everyone you know. Stop the slop.

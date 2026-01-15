# Stop the Slop

A Claude Code skill to strip AI writing patterns from prose. Makes text sound human.

## What It Does

Final-pass audit that catches AI tells your editing missed:

- **False Agency** — objects doing human verbs ("The data tells us")
- **Narrator Voice** — floating above the scene instead of putting the reader in it
- **Wh- Openers** — sentences starting with What/Why/How as a crutch
- **Vague Declaratives** — "The implications are significant" without naming them
- **Negative Runway** — "Not X. Not Y. It's Z." buildup
- **Three-Item Lists** — AI loves triplets. Humans use two.
- **Question Endings** — LinkedIn CTA energy
- **Over-Explanation** — defining terms readers already know
- **Adverb Infestation** — genuinely, fundamentally, truly, inevitably
- **Passive Hiding** — "Mistakes were made" instead of naming who

## Installation

Copy the `skill/` folder to your Claude Code skills directory:

```bash
cp -r skill/ ~/.claude/skills/stop-the-slop/
```

Or clone and symlink:

```bash
git clone https://github.com/yourname/stop-the-slop.git
ln -s $(pwd)/stop-the-slop/skill ~/.claude/skills/stop-the-slop
```

## Usage

After drafting and editing your content:

```
/stop-the-slop
```

The skill runs a final audit against all patterns. If anything fails, fix it and re-run.

## Workflow Position

```
Draft → Edit → Score 8/10+ → /stop-the-slop → Publish
```

This is a **final audit**, not a drafting tool. Run it after your content is polished, before publishing.

## The Test

Read it aloud.

- Sounds like explaining to a peer over coffee → **Pass**
- Sounds like a LinkedIn post → **Fix it**
- Sounds like performing expertise → **Fix it**

## License

MIT

# AUDHD Executive Function Skill

A Claude Code skill that turns AI into an external executive function system for people with AUDHD (combined ADHD + Autism).

## What it does

Your AI stops being an assistant. It becomes your working memory, your task initiator, your follow-up tracker, and your copywriter. You open one page each morning. Everything you need to do is there, pre-written, in order, ready to copy-paste.

**One rule: if you can't copy-paste it, click it, or check it off, it doesn't belong.**

## The problem it solves

AUDHD executive function deficits are specific and compounding:
- **Working memory** - if a task isn't on screen, it doesn't exist
- **Task initiation** - the Wall of Awful blocks starting, not finishing
- **Decision fatigue** - choosing what to do next burns more energy than doing it
- **Time blindness** - "this week" means nothing, "by 2:00 PM" works
- **RSD** - rejection sensitivity makes outreach and follow-ups feel dangerous

Traditional productivity tools assume you can hold context, switch tasks, and self-motivate. AUDHD brains can't reliably do any of those things. This skill doesn't ask you to try harder. It removes the need.

## How it works

The skill instructs Claude to generate a daily HTML workbench (not a briefing) with these properties:

**Every item has:**
- The actual text to send (in a copy box with a Copy button)
- A link to open the right page
- Time estimate
- Energy tag (Quick Win / Deep Focus / People / Admin)
- Inline context (who this person is, last interaction, what's owed)

**The system decides. You execute.**
- Who to contact (priority, cooling risk, pipeline health)
- What to say (pre-written in your voice)
- In what order (friction-sorted, easiest first)
- Through which channel (DM, email, comment)

**No shame. Ever.**
- "Carried forward" not "overdue"
- "Ready when you are" not "missed"
- Effort tracking ("you sent 4 messages") not outcome tracking ("0 replies")
- Skipped items move forward without commentary

## What's in the box

```
SKILL.md                          # The full skill definition
references/
  research.md                     # AUDHD research (Barkley, Mahan, Dodson, 30+ sources)
  assaf-profile.md                # Example user profile (customize for your own use)
```

## Installation

### Claude Code

Drop the folder into your project:

```
.claude/skills/audhd-executive-function/
```

Then reference it in your `CLAUDE.md`:

```markdown
## AUDHD Executive Function Rule (ENFORCED)

Every output the user will act on must follow the `audhd-executive-function` skill.
Read `.claude/skills/audhd-executive-function/SKILL.md` before generating any actionable output.
```

### Customization

1. Edit `references/assaf-profile.md` with your own patterns (what works, what fails, energy patterns)
2. The skill adapts to whatever tools and workflows you use. The rules are universal. The content is yours.

## Key design principles

| Principle | Why |
|---|---|
| **Zero decisions to start** | Decision fatigue is real. System picks the best action. You override if you want. |
| **Momentum-first ordering** | Quick Wins first. Build dopamine. Then harder tasks. Never start with the hardest item. |
| **Single surface** | One page. No switching tools, tabs, or apps. |
| **Copy-paste ready** | Every message is final-draft quality. No blank-page paralysis. |
| **Independent sections** | Skipping one section never breaks another. "3 of 7 done" is a win. |
| **Automatic crack detection** | System surfaces what fell through. You never have to remember to check. |
| **No pressure language** | Words like "overdue," "missed," "urgent" trigger freeze. Banned entirely. |

## Research foundation

Built on:
- **Barkley** - external scaffolding as executive function replacement
- **Mahan** - Wall of Awful framework and emotional barrier mitigation
- **Dodson** - interest-based nervous system, RSD
- 30+ additional sources from PMC, Nature, CHADD, ADDitude, Cleveland Clinic, ADDA

Full research synthesis in `references/research.md`.

## Who this is for

Anyone with ADHD, ASD, or AUDHD who uses Claude Code for work and needs their AI to do more than answer questions. It needs to run your day.

Built by a founder with AUDHD who got tired of productivity systems designed for neurotypical brains.

## License

MIT

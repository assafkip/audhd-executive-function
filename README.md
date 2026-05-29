# AUDHD Executive Function Skill for Claude Code

A free Claude Code skill that turns your AI into an external executive function system for people with AUDHD (combined ADHD + Autism). It is the working memory, task initiator, follow-up tracker, and copywriter you stop having to be.

**One rule: if you cannot copy-paste it, click it, or check it off, it does not belong in the output.**

Install it in 30 seconds:

```
.claude/skills/audhd-executive-function/
```

Then add one block to your `CLAUDE.md` (full instructions below) and ask Claude to generate your daily schedule. Every item comes back copy-paste ready, friction-sorted, with a time estimate and an energy tag.

_Version 1.1 - updated 2026-05-28. MIT licensed. Works with Claude Code (any project)._

## What is the AUDHD Executive Function skill?

It is a skill file (`SKILL.md`) plus a research base and a profile template. When loaded, it changes how Claude structures every actionable output. Instead of giving you a briefing, a dashboard, or a list of options to evaluate, Claude produces a single daily HTML workbench where:

- Every message is pre-written in your voice, in a copy box with a Copy button
- Every item has a link to open the right page, a time estimate, and an energy tag (Quick Win / Deep Focus / People / Admin)
- The system decides who to contact, what to say, in what order, through which channel
- You only copy, click, paste, and check off

The skill is generic. You fill in a local profile (your tools, your voice, your patterns) and it adapts to your work.

## How do I stop my AI from giving me dashboards instead of actions?

This is the core problem the skill solves. Most AI output is informational: scores, summaries, "you have 8 hot prospects." For an AUDHD brain, a number without an attached next step is noise that burns decision energy.

The skill enforces hard anti-patterns. No dashboard without an attached draft. No pipeline count without a per-person action. No "see section above." No options to evaluate. If a section has zero actions, it gets omitted. Dashboards live in a collapsed block at the bottom, and every dashboard row must link to an action above it or it does not get rendered.

The result is a single surface where the top of the page is only things you can do right now.

## Why do productivity tools fail for ADHD and autistic brains?

Traditional productivity tools assume you can hold context, switch tasks, and self-motivate. AUDHD executive function deficits make all three unreliable:

- **Working memory:** if a task is not on screen, it does not exist
- **Task initiation:** the Wall of Awful blocks starting, not finishing
- **Decision fatigue:** choosing the next action burns more energy than doing it
- **Time blindness:** "this week" means nothing, "by 2:00 PM" works
- **RSD:** rejection sensitivity makes outreach and follow-ups feel dangerous

This skill does not ask you to try harder. It removes the need. It pre-processes the emotional labor (all messages written, all outreach framed as sharing value), orders by momentum (Quick Wins first to build dopamine), and never uses pressure or shame language.

## How is this different from a normal task manager or Notion template?

| Normal task manager | This skill |
|---|---|
| You write the tasks | The system writes them, pre-filled with the actual text to send |
| Lists what to do | Lists the literal next physical action, copy-paste ready |
| You decide priority order | Friction-sorted, easiest first, momentum-first |
| "Overdue" and red flags | "Carried forward," no shame language, ever |
| Multiple tabs and tools | One HTML page, single surface, works on phone |
| Tracks outcomes (0 replies) | Tracks effort (you sent 4 messages) |
| You remember to check follow-ups | Automatic crack detection surfaces what fell through |

It is not a replacement for your CRM or your calendar. It is the layer on top that turns their data into a workday you can execute action by action.

## How do I install and use it?

### 1. Install

Drop the folder into your project:

```
.claude/skills/audhd-executive-function/
```

### 2. Tell Claude to use it

Add this to your `CLAUDE.md`:

```markdown
## AUDHD Executive Function Rule (ENFORCED)

Every output the user will act on must follow the `audhd-executive-function` skill.
Read `.claude/skills/audhd-executive-function/SKILL.md` before generating any actionable output.
```

### 3. Make it yours

Open `references/user-profile.md`. It is a template with prompts. Fill in what works for you, what makes you freeze, your energy patterns, your tools, and your voice (paste 2-3 real messages so the system writes like you). This file stays local. Nobody sees it but your AI.

### 4. Start using it

Ask Claude to generate your daily schedule. It reads the skill, reads your profile, and produces an HTML workbench where every item is copy-paste ready.

## What is in the repo?

```
SKILL.md                 The full skill definition (generic, ready to use)
references/
  research.md            AUDHD research base (Barkley, Mahan, Dodson, 30+ sources)
  user-profile.md        Template - fill in your own patterns, tools, and voice
LICENSE                  MIT
```

## What research is this built on?

- **Barkley** - external scaffolding as executive function replacement
- **Mahan** - the Wall of Awful framework and emotional barrier mitigation
- **Dodson** - interest-based nervous system and RSD
- 30+ additional sources from PMC, Nature, CHADD, ADDitude, Cleveland Clinic, and ADDA

Full synthesis in `references/research.md`. The design principles map directly to documented deficits: zero decisions to start, single surface, copy-paste ready, energy-aware batching, progress visibility, no shame language, automatic crack detection, and inline relationship memory.

## Who is this for?

Anyone with ADHD, ASD, or AUDHD who uses Claude Code for work and needs their AI to do more than answer questions. It needs to run the day.

Built by a founder with AUDHD who got tired of productivity systems designed for neurotypical brains.

## License

MIT. See [LICENSE](LICENSE).

---

I built this AUDHD executive function skill for my own work and open-sourced the free version here.

If you want the full playbook (the complete system, the daily HTML workbench spec, the voice and profile setup walked through end to end), I packaged it as the **AUDHD Executive Function Playbook ($39)**: https://claudedaddy.gumroad.com/l/isekq

More Claude Code kits for founders: https://claudedaddy.gumroad.com

Want one wired to your own setup? Book a call: https://calendar.app.google/cMFvhvDsfi9iyWYy9

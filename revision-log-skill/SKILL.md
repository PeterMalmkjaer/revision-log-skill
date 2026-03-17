---
name: revision-log
description: Helps track what worked, what failed, and why decisions were made — so you can learn from a project and recreate it. Use this skill when the user mentions a log, changelog, audit trail, revision history, "what did I do", "why did I do this", "I want to remember how I solved this", or "I want to turn this experience into a skill". Also use when wrapping up a session, reviewing a project, or building documentation from experience. Works for any iterative project — software, writing, research, data analysis, or design.
---

# Revision Log — Tracking What Worked, What Failed, and Why

A skill for maintaining a log that lets you reconstruct decisions, learn from mistakes, and transfer knowledge.
Principle: **A log records decisions, not just actions. Anyone (including future you) should be able to read it and understand why.**

---

## The Core Problem

Most project logs fail in one of three ways:
1. **Only records what was done** — not why, not what failed first
2. **Written at the end** — reconstructed from memory, misses the real sequence
3. **Too detailed or too sparse** — either unreadable or useless

The goal is a log that answers: *"What was tried, what worked, what did not, and what was decided?"*

---

## Log Entry Structure

Every entry has four elements:

```
## YYYY-MM-DD — Session/version label

### Done
- What was actually completed (specific: file names, version numbers, counts)

### Decisions made
- WHY something was done a certain way (not just what)
- Alternatives that were considered and rejected — and why
- Constraints that shaped the decision

### Problems encountered
- What went wrong
- How it was diagnosed
- How it was resolved (or: why it was accepted/deferred)

### Status
- Current state in one sentence
- Next step
```

---

## What Makes a Good Log Entry

**Good — records decision and reasoning:**
> "Changed chapter template to add perspective box after learning goals. Previous version had it before, which meant students saw the summary before the content — pedagogically wrong. Considered removing it entirely but kept it as a navigation aid."

**Bad — records only action:**
> "Updated chapter template."

---

**Good — records failure and resolution:**
> "overfull hbox 185pt on Appendix D title. Caused by long title in 24pt font without line break. Fixed with chapter[short]{long continued} pattern. Rejected linebreak inside title as it breaks TOC."

**Bad — records only fix:**
> "Fixed appendix title."

---

## The WHAT / WHY / WHAT-FAILED Framework

For every significant change, log three things:

| Element | Question | Example |
|---------|---------|---------|
| **WHAT** | What exactly changed? | "Reference count: 150 T1, 32 T2 to 182 T1, 0 T2" |
| **WHY** | Why this approach? | "T2 references were unverifiable from memory alone — required primary source check" |
| **WHAT FAILED** | What was tried first? | "Tried batch upgrade from LLM knowledge — rejected: violates verification standard" |

---

## Turning a Log into a Skill

When a project is complete, a good log contains everything needed to build a reusable skill:

1. **Read the log** — identify recurring patterns (what was done repeatedly)
2. **Extract the decisions** — what choices were made and why (these become the skill's principles)
3. **Extract the failures** — what went wrong (these become the skill's warnings)
4. **Extract the procedures** — what steps were followed (these become the skill's templates)
5. **Generalise** — remove project-specific details, keep the pattern

Example: The PM-book project log contained entries about backup failures, numbering mistakes, and reference verification problems. Those entries became Templates 3, 7, and 8 in the academic-book skill.

---

## Log Levels

| Level | When | Format |
|-------|------|--------|
| **Minimal** | Short projects, solo work | One bullet per session: date + done + next |
| **Standard** | Multi-week projects | Done + decisions + problems per session |
| **Full** | Long projects, team work, or "will become a skill" | Complete WHAT/WHY/WHAT-FAILED per change |

---

## Anti-Patterns to Avoid

| Anti-pattern | Why it fails | Fix |
|-------------|-------------|-----|
| "Fixed bug" | No context for future reader | "Fixed overfull 185pt by adding line break — caused by 50-char title in 24pt font" |
| Logging only successes | Failures contain the real learning | Always log what was tried first |
| Retrospective logging | Memory distorts sequence and reasons | Log during the session, not after |
| Private shorthand | Unreadable in 6 months | Write for a reader who was not there |
| Separate log from project | Log gets lost | Keep log file in the project folder |

---

## Starter Template

Copy this into your project folder as `LOG.md`:

```markdown
# Project Log

---

## YYYY-MM-DD — Label

### Done
-

### Decisions
-

### Problems
-

### Status
- Current state:
- Next:
```

---

**Single most important rule:** Log the reason, not just the action. The action is visible in the files. The reason exists only in the log.

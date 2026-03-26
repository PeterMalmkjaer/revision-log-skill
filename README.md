# revision-log-skill

A Claude Cowork skill for tracking what worked, what failed, and why decisions were made — so you can learn from a project and recreate it.

**Beta — v0.2**

Universal: works for any iterative project — software, writing, research, data analysis, or design.

## Core principle

A log records **decisions**, not just actions. The action is visible in the files. The reason exists only in the log.

## What it covers

- Log entry structure: Done / Decisions / Problems / Status
- The WHAT / WHY / WHAT-FAILED framework
- How to turn a project log into a reusable skill
- **NEW:** Turning a project log into a formal report (Log to Report workflow)
- Log levels (minimal / standard / full)
- Practical formats (Markdown, spreadsheet)
- Anti-patterns to avoid
- Starter template (copy-paste ready)

## Log to Report workflow (NEW in v0.2)

A detailed project log is not just an internal record — it is the raw material for a formal report, a methodology section, or an article about the process itself.

**The five-step process:**

1. **Read the full log** — not a summary. The log contains decisions, failures, and pivots that a summary would omit.
2. **Extract the structure** — identify natural phases or stages. These become the report sections.
3. **Quantify** — count everything: items checked, errors found, types, percentages.
4. **Classify and reflect** — group findings into categories. What patterns emerge? What required human judgement?
5. **Write the report** — Scope, Method, Results, Analysis, Reflection, Appendices.

The log records events bottom-up. The report tells a story top-down. The transformation requires identifying the narrative thread connecting individual entries.

**Practical tip:** Generate the report programmatically (docx-js or python-docx) for professional formatting with tables and headers.

*Developed during a 28-phase source verification project where a 2,156-line log became a 9-section .docx report.*

---

## License

MIT — Peter Malmkjaer, CBS, 2026. Updated March 26, 2026.

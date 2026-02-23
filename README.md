# vc-pe-toolkit

A community-driven collection of [Claude Skills](https://support.anthropic.com) for private equity and venture capital workflows.

## What this is

PE and VC professionals spend a lot of time on tasks that are repetitive but high-stakes — CIM teardowns, portfolio monitoring, deal screening, LP reporting. Claude Skills can automate meaningful chunks of that work, but most teams are building them in isolation.

This repository is an open toolkit. The idea is simple: contribute a skill that saves you time, and get access to dozens of others that do the same.

## Skills

| Skill | Category | Description |
|-------|----------|-------------|
| [Pitch Deck Triage](/skills/pitch-deck-triage) | Sourcing & screening | Structured teardown of inbound pitch decks. Extracts financials, team, timing thesis, and deal terms. Flags gaps, surfaces questions, finds comps (including dead ones). IC-ready summary + full analysis. |

> **Looking for a specific workflow?** Open an [issue](../../issues) and describe what you're trying to automate. Chances are someone else needs it too.

## Categories

Skills are organized by where they sit in the investment lifecycle:

- **Sourcing & screening** — market scans, target identification, initial filtering
- **Due diligence** — CIM analysis, financial model review, risk flagging
- **Deal execution** — term sheet comparison, document generation, data room review
- **Portfolio monitoring** — KPI dashboards, reporting templates, covenant tracking
- **Fundraising & IR** — LP reporting, fund performance summaries, DDQ responses
- **Back office** — compliance checks, document formatting, data extraction

## Contributing

We welcome contributions from anyone working in PE, VC, growth equity, or adjacent fields.

### How to submit a skill

1. Fork this repository
2. Create a folder under `/skills/` with a descriptive name (e.g., `cim-analyzer`)
3. Include:
   - `SKILL.md` — the skill instructions Claude should follow
   - `README.md` — a brief description of what it does, when to use it, and any setup notes
   - Sample files or templates if applicable
4. Open a pull request with a short summary of the use case

### Guidelines

- **Keep skills focused.** One skill, one job. A skill that extracts key terms from an LPA is better than one that tries to do all of legal review.
- **Be specific about inputs and outputs.** What file types does it expect? What does the user get back?
- **Test before submitting.** If it works reliably in your workflow, it's ready.
- **No proprietary data.** Use synthetic or anonymized examples only.

## Using these skills

Each skill folder contains a `SKILL.md` file with the full prompt. To use one:

1. Navigate to the skill you need
2. Copy the contents of `SKILL.md`
3. Add it to your Claude project as a custom skill or paste it into your system prompt
4. Follow the skill's README for any setup steps

Detailed setup instructions are in each skill's folder.

## Why open source this

Most PE/VC teams are building AI workflows behind closed doors, which makes sense for proprietary strategy — but not for operational tooling. The mechanics of parsing a CIM or formatting an LP report are not competitive advantages. Sharing them makes everyone faster.

## License

[MIT](LICENSE) — use these skills however you want, commercially or otherwise.

## Stay in the loop

New skills, demos of vibe-coded tools for IPs and portfolio companies, and playbooks that actually get used. People in the space share what's working. Mails sent when ready, not on a schedule.

→ [pevctoolkit on Buttondown](https://buttondown.com/pevctoolkit)

## Related

- [Anthropic Documentation](https://docs.anthropic.com) — API reference and prompting guides
- [Claude Skills Guide](https://support.anthropic.com) — how skills work in Claude

---

**Have a skill that saves your team hours every week?** [Open a PR](../../pulls) and share it.

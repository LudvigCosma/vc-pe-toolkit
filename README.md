<p align="center">
  <img src="assets/banner.svg" alt="VC/PE Toolkit — Open-source AI skills for private equity and venture capital" width="100%">
</p>

<p align="center">
  <a href="#skills"><img src="https://img.shields.io/badge/Skills-6-blue?style=flat-square" alt="Skills"></a>
  <a href="#contributing"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen?style=flat-square" alt="PRs Welcome"></a>
  <a href="https://github.com/LudvigCosma/vc-pe-toolkit/issues/new?template=submit-skill.yml"><img src="https://img.shields.io/badge/Submit_a_Skill-blue?style=flat-square&logo=github" alt="Submit a Skill"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow?style=flat-square" alt="License: MIT"></a>
  <a href="https://www.linkedin.com/in/ludvig-st%C3%A5lberg-cosma/"><img src="https://img.shields.io/badge/LinkedIn-Follow-0A66C2?style=flat-square&logo=linkedin" alt="LinkedIn"></a>
</p>

---

## What are Agent Skills?

Agent Skills are portable instructions that teach AI agents how to perform specific tasks your way. For PE and VC professionals, this means encoding your expertise into reusable AI workflows. Tear down CIMs using your firm's methodology. Screen pitch decks against your investment criteria. Generate LP reports in your format.

Write once, use anywhere — skills are an open standard with growing adoption across AI platforms.

<p align="center">
  <img src="https://img.shields.io/badge/Claude-Works-f97316?style=for-the-badge&logo=anthropic&logoColor=white" alt="Claude">
  &nbsp;
  <img src="https://img.shields.io/badge/OpenAI-Works-412991?style=for-the-badge&logo=openai&logoColor=white" alt="OpenAI">
  &nbsp;
  <img src="https://img.shields.io/badge/Gemini-Works-4285F4?style=for-the-badge&logo=google&logoColor=white" alt="Gemini">
</p>

---

## Browse

<p align="center">
  <img src="assets/categories.svg" alt="Skill categories" width="100%">
</p>

| # | Category | Focus Area |
|---|----------|------------|
| [01](#sourcing--screening) | **Sourcing & Screening** | Deal screening, target identification, initial filtering |
| [02](#due-diligence) | **Due Diligence** | CIM analysis, financial model review, risk flagging |
| [03](#deal-execution) | **Execution** | Term sheet comparison, document generation, data room review |
| [04](#portfolio-monitoring) | **Monitoring** | KPI dashboards, reporting templates, covenant tracking |
| [05](#fundraising--ir) | **Fundraising & IR** | LP reporting, fund performance summaries, DDQ responses |
| [06](#back-office) | **Back Office** | Compliance checks, document formatting, data extraction |
| [07](#legal) | **Legal** | Contract review, NDA triage, legal risk assessment |
| [08](#meta-skills) | **Meta Skills** | Skill creation, optimization, orchestration |

---

## Skills

### Sourcing & Screening

> **[Pitch Deck Triage](skills/pitch-deck-triage)** &nbsp; · &nbsp; *by [LudvigCosma](https://github.com/LudvigCosma)*

*Structured teardown of inbound pitch decks. Extracts financials, team, timing thesis, and deal terms. Flags gaps, surfaces questions, finds comps (including dead ones). IC-ready summary + full analysis.*

<img src="assets/divider.svg" width="100%">

### Due Diligence

*No skills yet — [submit one!](https://github.com/LudvigCosma/vc-pe-toolkit/issues/new?template=submit-skill.yml)*

<img src="assets/divider.svg" width="100%">

### Legal

> **[Contract Review](contract-review-anthropic)** &nbsp; · &nbsp; *by [LudvigCosma](https://github.com/LudvigCosma)*

*Reviews commercial contracts clause-by-clause. Identifies risk areas, missing protections, and non-standard terms. Produces a structured issue log with severity ratings and suggested redline language.*

> **[NDA Triage](nda-triage-anthropic)** &nbsp; · &nbsp; *by [LudvigCosma](https://github.com/LudvigCosma)*

*Screens incoming NDAs and classifies them by risk level. Flags non-standard clauses, carve-out gaps, and jurisdiction issues. Outputs a quick assessment with recommended actions.*

> **[Legal Risk Assessment](legal-risk-assessment-anthropic)** &nbsp; · &nbsp; *by [LudvigCosma](https://github.com/LudvigCosma)*

*Evaluates legal risk across transaction documents. Maps regulatory exposure, identifies liability concentrations, and produces a risk matrix with mitigation recommendations.*

<img src="assets/divider.svg" width="100%">

### Back Office

> **[Compliance Check](compliance-anthropic)** &nbsp; · &nbsp; *by [LudvigCosma](https://github.com/LudvigCosma)*

*Runs compliance screening workflows. Checks regulatory requirements, flags potential issues, and generates compliance reports with action items.*

<img src="assets/divider.svg" width="100%">

### Deal Execution

*No skills yet — [submit one!](https://github.com/LudvigCosma/vc-pe-toolkit/issues/new?template=submit-skill.yml)*

### Portfolio Monitoring

*No skills yet — [submit one!](https://github.com/LudvigCosma/vc-pe-toolkit/issues/new?template=submit-skill.yml)*

### Fundraising & IR

*No skills yet — [submit one!](https://github.com/LudvigCosma/vc-pe-toolkit/issues/new?template=submit-skill.yml)*

### Meta Skills

*No skills yet — [submit one!](https://github.com/LudvigCosma/vc-pe-toolkit/issues/new?template=submit-skill.yml)*

---

## Get Started

Each skill folder contains a `SKILL.md` file with the full prompt. To use one:

1. Navigate to the skill you need
2. Copy the contents of `SKILL.md`
3. Add it to your AI agent as a custom skill or system prompt
4. Follow the skill's `README.md` for any setup steps

> [!TIP]
> Skills work across platforms. While they're optimized for Claude, most work well with any capable AI agent.

---

## Contributing

We welcome contributions from anyone working in PE, VC, growth equity, or adjacent fields.

### Quick Submit (no Git required)

**[Submit a Skill here!](https://github.com/LudvigCosma/vc-pe-toolkit/issues/new?template=submit-skill.yml)** — Fill out the form and we'll handle the rest.

### Submit via Pull Request

1. Fork this repository
2. Create a folder under `/skills/` with a descriptive name (e.g., `lpa-term-extractor`)
3. Include:
   - `SKILL.md` — the skill instructions the AI agent should follow
   - `README.md` — what it does, when to use it, any setup notes
   - Sample files or templates if applicable
4. Open a pull request with a short summary of the use case

### Quality Guidelines

- **Focused** — One skill, one job. A skill that extracts key terms from an LPA is better than one that tries to do all of legal review.
- **Specific** — Be clear about inputs and outputs. What file types does it expect? What does the user get back?
- **Tested** — If it works reliably in your workflow, it's ready.
- **Clean** — No proprietary data. Use synthetic or anonymized examples only.

> [!NOTE]
> All submissions are reviewed for quality and security before being added to the list.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the full guide.

---

## Why Open Source This?

Most PE/VC teams are building AI workflows behind closed doors, which makes sense for proprietary strategy — but not for operational tooling. The mechanics of parsing a CIM or formatting an LP report are not competitive advantages. Sharing them makes everyone faster.

---

## Stay in the Loop

New skills, demos, and playbooks that actually get used. Mails sent when ready, not on a schedule.

**[Subscribe on Buttondown](https://buttondown.com/pevctoolkit)**

---

## Related Resources

- [Anthropic Documentation](https://docs.anthropic.com) — API reference and prompting guides
- [Claude Skills Guide](https://docs.anthropic.com/en/docs/agents-and-tools/claude-code/skills) — How skills work in Claude
- [awesome-legal-skills](https://github.com/lawvable/awesome-legal-skills) — Curated AI skills for legal work

---

## License

[MIT](LICENSE) — use these skills however you want, commercially or otherwise.

---

<p align="center">
  <sub>Have a skill that saves your team hours every week? <a href="https://github.com/LudvigCosma/vc-pe-toolkit/issues/new?template=submit-skill.yml">Submit it</a> and share it with the community.</sub>
</p>

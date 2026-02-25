# Contributing to VC/PE Toolkit

We welcome contributions from anyone working in PE, VC, growth equity, or adjacent fields. Whether you've built a skill that saves your team hours or have an idea for one, here's how to get involved.

## Two Ways to Submit

### 1. Quick Submit (no Git required)

**[Use the submission form](https://github.com/LudvigCosma/vc-pe-toolkit/issues/new?template=submit-skill.yml)** — fill out the fields, attach your skill file, and we'll handle the rest. No Git knowledge needed.

### 2. Pull Request

1. **Fork** this repository
2. **Create a folder** under `/skills/` with a descriptive, kebab-case name (e.g., `lpa-term-extractor`)
3. **Include these files:**
   - `SKILL.md` — the complete skill instructions the AI agent should follow
   - `README.md` — a brief description of what it does, when to use it, and any setup notes
   - Sample files or templates if applicable (use synthetic data only)
4. **Open a pull request** with a short summary of the use case

## Skill Structure

```
skills/
└── your-skill-name/
    ├── SKILL.md          # The actual skill prompt
    ├── README.md         # Documentation
    └── examples/         # Optional: sample inputs/outputs
        ├── sample-input.pdf
        └── sample-output.md
```

## Quality Standards

### Keep it focused
One skill, one job. A skill that extracts key terms from an LPA is better than one that tries to do all of legal review.

### Be specific about I/O
What file types does it expect? What does the user get back? Be explicit about inputs and outputs.

### Test before submitting
If it works reliably in your workflow, it's ready. Mention which platform you tested on (Claude, OpenAI, Gemini, etc.).

### No proprietary data
Use synthetic or anonymized examples only. Never include real company names, financials, or confidential information.

## Review Process

All submissions go through a review before being added:

1. **Quality check** — Does it do what it says? Is the prompt well-structured?
2. **Security screening** — No malicious instructions, data exfiltration, or harmful patterns
3. **Uniqueness** — Does it add something the toolkit doesn't already have?
4. **Documentation** — Is it clear how to use it?

We aim to review submissions within a few days. You'll get feedback in the issue or PR comments.

## Categories

Skills are organized by where they sit in the investment lifecycle:

| Category | Description |
|----------|-------------|
| Sourcing & Screening | Market scans, target identification, initial filtering |
| Due Diligence | CIM analysis, financial model review, risk flagging |
| Deal Execution | Term sheet comparison, document generation, data room review |
| Portfolio Monitoring | KPI dashboards, reporting templates, covenant tracking |
| Fundraising & IR | LP reporting, fund performance summaries, DDQ responses |
| Back Office | Compliance checks, document formatting, data extraction |
| Legal | Contract review, NDA triage, legal risk assessment |
| Meta Skills | Skill creation, optimization, orchestration |

## Code of Conduct

Be respectful, be constructive. This is a professional community — treat contributions and contributors accordingly.

## Questions?

Open an [issue](https://github.com/LudvigCosma/vc-pe-toolkit/issues) or reach out on [LinkedIn](https://www.linkedin.com/in/ludvig-st%C3%A5lberg-cosma/).

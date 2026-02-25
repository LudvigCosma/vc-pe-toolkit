# Contributing to VC/PE Toolkit

We welcome contributions from anyone working in PE, VC, growth equity, or adjacent fields. Whether you've built a skill, workflow, or playbook that saves your team time, here's how to get involved.

## What You Can Submit

| Type | What It Is | Example |
|------|-----------|---------|
| **Skill** | A `SKILL.md` that an AI agent can follow to complete a specific task | CIM teardown prompt for Claude |
| **Workflow** | A step-by-step playbook for using AI tools to accomplish a goal | Using Gemini to process industry books during DD |
| **Template** | Reusable output formats, report structures, or analysis frameworks | IC memo template with AI-generated sections |

Resources can target any platform — Claude, Cowork, Gemini, OpenAI, or a combination.

## Two Ways to Submit

### 1. Quick Submit (no Git required)

**[Use the submission form](https://github.com/LudvigCosma/vc-pe-toolkit/issues/new?template=submit-resource.yml)** — fill out the fields, attach your files, and we'll handle the rest. No Git knowledge needed.

### 2. Pull Request

1. **Fork** this repository
2. **Create a folder** with a descriptive, kebab-case name (e.g., `gemini-book-dd`, `lpa-term-extractor`)
3. **Include these files:**
   - `SKILL.md` or `WORKFLOW.md` — the core instructions or playbook
   - `README.md` — what it does, when to use it, which tools are required
   - Sample files or templates if applicable (use synthetic data only)
4. **Open a pull request** with a short summary of the use case

## Folder Structure

### For Skills
```
skills/
└── your-skill-name/
    ├── SKILL.md          # The actual skill prompt
    ├── README.md         # Documentation
    └── examples/         # Optional: sample inputs/outputs
```

### For Workflows
```
workflows/
└── your-workflow-name/
    ├── WORKFLOW.md       # Step-by-step playbook
    ├── README.md         # Overview and prerequisites
    └── templates/        # Optional: output templates, prompts
```

## Quality Standards

### Keep it focused
One resource, one job. A skill that extracts key terms from an LPA is better than one that tries to do all of legal review.

### Be specific about I/O
What inputs does it expect? What does the user get back? Which tools are needed? Be explicit.

### Specify the platform
Mention which platform(s) you've tested on — Claude, Cowork, Gemini, OpenAI, etc. If it's platform-agnostic, say so.

### Test before submitting
If it works reliably in your workflow, it's ready.

### No proprietary data
Use synthetic or anonymized examples only. Never include real company names, financials, or confidential information.

## Review Process

All submissions go through a review before being added:

1. **Quality check** — Does it do what it says? Is the prompt or workflow well-structured?
2. **Security screening** — No malicious instructions, data exfiltration, or harmful patterns
3. **Uniqueness** — Does it add something the toolkit doesn't already have?
4. **Documentation** — Is it clear how to use it and what tools are needed?

We aim to review submissions within a few days. You'll get feedback in the issue or PR comments.

## Categories

Resources are organized by where they sit in the investment lifecycle:

| Category | Description |
|----------|-------------|
| Sourcing & Screening | Market scans, target identification, initial filtering |
| Due Diligence | CIM analysis, financial model review, market research, risk flagging |
| Deal Execution | Term sheet comparison, document generation, data room review |
| Portfolio Monitoring | KPI dashboards, reporting templates, covenant tracking |
| Fundraising & IR | LP reporting, fund performance summaries, DDQ responses |
| Back Office | Compliance checks, document formatting, data extraction |
| Legal | Contract review, NDA triage, legal risk assessment |
| Meta | Skill creation, workflow design, optimization |

## Code of Conduct

Be respectful, be constructive. This is a professional community — treat contributions and contributors accordingly.

## Questions?

Open an [issue](https://github.com/LudvigCosma/vc-pe-toolkit/issues) or reach out on [LinkedIn](https://www.linkedin.com/in/ludvig-st%C3%A5lberg-cosma/).

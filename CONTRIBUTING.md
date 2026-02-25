# Contributing to VC/PE Toolkit

We welcome contributions from anyone working in PE, VC, growth equity, or adjacent fields. Whether you've built a skill, discovered a useful tool, or know of an MCP server that belongs here — here's how to get involved.

## What You Can Submit

| Type | What It Is | What to Include | Example |
|------|-----------|-----------------|---------|
| **Tool Suggestion** | An AI-native tool PE/VC teams should know about | Name, URL, description, category | Relationship intelligence CRM for dealmakers |
| **MCP Server** | An MCP server useful for investment workflows | GitHub repo URL, description, what it connects to | Server for querying SEC EDGAR filings |
| **Skill** | A `SKILL.md` that an AI agent can follow | SKILL.md file, README, examples | CIM teardown prompt for Claude |
| **Workflow** | A step-by-step playbook for using AI tools | WORKFLOW.md, prerequisites, sample outputs | Using Gemini to process industry books during DD |
| **Playbook** | End-to-end guide combining tools, MCPs, and skills | Markdown guide with setup steps | Complete AI-powered DD research workflow |
| **Template** | Reusable output formats or analysis frameworks | Template file, usage instructions | IC memo template with AI-generated sections |

## Two Ways to Submit

### 1. Quick Submit (no Git required)

**[Use the submission form](https://github.com/LudvigCosma/vc-pe-toolkit/issues/new?template=submit-resource.yml)** — fill out the fields, and we'll handle the rest. No Git knowledge needed.

This is the best option for:
- **Tool suggestions** — just provide the name, URL, and a short description
- **MCP server recommendations** — link the GitHub repo and explain the use case
- **Quick skill or playbook submissions** — attach your files directly

### 2. Pull Request

1. **Fork** this repository
2. **For skills:** create a folder under `skills/` with a descriptive, kebab-case name (e.g., `cim-teardown`, `lpa-term-extractor`)
3. **For tools/MCPs:** no folder needed — add entries to the relevant table in `README.md`
4. **For playbooks:** create a folder under `playbooks/` with a descriptive name
5. **Include these files** (for skills/playbooks):
   - `SKILL.md` or `PLAYBOOK.md` — the core instructions
   - `README.md` — what it does, when to use it, which tools are required
   - Sample files or templates if applicable (use synthetic data only)
6. **Open a pull request** with a short summary of the use case

## Folder Structure

### For Skills
```
skills/
└── your-skill-name/
    ├── SKILL.md          # The actual skill prompt
    ├── README.md         # Documentation
    └── examples/         # Optional: sample inputs/outputs
```

### For Playbooks
```
playbooks/
└── your-playbook-name/
    ├── PLAYBOOK.md       # End-to-end guide
    ├── README.md         # Overview and prerequisites
    └── templates/        # Optional: output templates
```

### For Tools & MCP Servers

No folder needed. Submit via issue form or add directly to the relevant table in `README.md` via PR.

## Quality Standards

### Keep it focused
One resource, one job. A skill that extracts key terms from an LPA is better than one that tries to do all of legal review.

### Be specific about I/O
What inputs does it expect? What does the user get back? Which tools are needed? Be explicit.

### Test before submitting
If it works reliably in your workflow, it's ready.

### No proprietary data
Use synthetic or anonymized examples only. Never include real company names, financials, or confidential information.

### For tool/MCP suggestions
- Include the tool name and URL
- Write a concise description (1-2 sentences) of what it does and why it's relevant to PE/VC
- Specify the category it fits into

## Categories

Resources are organized into four pillars:

| Pillar | Subcategories |
|--------|---------------|
| **Tools Directory** | Deal CRMs, Deal Sourcing, Due Diligence, Portfolio Monitoring, Data Rooms, LP Reporting, Market Intelligence, Value Creation |
| **MCP Servers** | Financial Data, Research & Web, Documents & Files, Productivity |
| **Skills & Workflows** | Community Skills, Anthropic Cowork Skills, Anthropic Cowork Plugins |
| **Playbooks** | End-to-end workflow guides |

## Review Process

All submissions go through a review before being added:

1. **Quality check** — Does it do what it says? Is the description accurate?
2. **Security screening** — No malicious instructions, data exfiltration, or harmful patterns
3. **Uniqueness** — Does it add something the toolkit doesn't already have?
4. **Documentation** — Is it clear how to use it and what tools are needed?

We aim to review submissions within a few days. You'll get feedback in the issue or PR comments.

## Code of Conduct

Be respectful, be constructive. This is a professional community — treat contributions and contributors accordingly.

## Questions?

Open an [issue](https://github.com/LudvigCosma/vc-pe-toolkit/issues) or reach out on [LinkedIn](https://www.linkedin.com/in/ludvig-st%C3%A5lberg-cosma/).

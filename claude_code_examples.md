# Claude Code Usage Examples from My Blog

A reference of concrete ways I've used Claude Code, drawn from blog posts — organized by how they expand my work.

---

## Going Deeper as a Data Scientist

Uses that make me more effective at the core craft of ML/data science.

### Agentic ML Workflows

Built an `agentic-ml-plugin` with 10 skills for running ML experiments end-to-end:

`review-target`, `plan-experiment`, `build-baseline`, `check-dataset-quality`, `check-data-pipeline`, `feature-engineering`, `babysit-training`, `check-failed-run`, `check-eval`, `explain-model`

Can orchestrate the full pipeline with a single command:
```
/orchestrate-e2e on the medium dataset in demo/
```

Also built `mlscribe`, a CLI tool to generate executable demonstration documents of agent work.

*Source: [Agentic Knowledge Work & Machine Learning](https://lawrencewu.net/posts/2026-03-04-agentic-knowledge-work/)*

### ML Model Improvement with autoresearch (2026)

Used Claude Code with Karpathy's `autoresearch` tool to improve ML models at UKG:

- Achieved **15–20% model improvements** on models I'd worked on for months
- autoresearch runs short training loops (50–100 experiments) with agentic reasoning to discover parameter tuning improvements
- Previously hadn't attempted this optimization because of the cognitive load and time burden

*Source: [autoresearch is a Claude Code Killer App](https://lawrencewu.net/posts/2026-03-27-autoresearch-cc-killer-app/)*

### Code & Data Exploration

- Uses `gh` CLI via Claude Code to understand new codebases (prefers this over GitHub MCP)
- Explores BigQuery data sources using `bq` CLI

*Source: [Year in Review 2025](https://lawrencewu.net/posts/2025-12-31-year-in-review/)*

---

## Broader in Data Science-Adjacent Fields

Uses that stretch into software engineering, MLOps, and tooling — skills adjacent to but outside core data science.

### Building Internal Tools (July 2025)

During a July 4th PTO week:

- **FastHTML web app** (internal company tool): estimated 2–3 days of work completed in <2 hours with ~5 prompts. Claude Code figured out how to combine FastHTML and FastAPI since both are Starlette apps.
- **MCP Server with FastMCP + bearer token auth**: also completed in <2 hours vs. an estimated 2–3 days.

*Source: [Starting to Use Claude Code](https://lawrencewu.net/posts/2025-07-18-starting-to-use-claude-code/)*

### Open Source MCP Server (mcp-lightcast)

- Built a Python SDK for the Lightcast API
- Identified a common workflow: normalizing job titles and retrieving related skills (normally 3 separate API calls)
- Created a dedicated MCP tool bundling those 3 calls for better agent efficiency
- Open-sourced as `mcp-lightcast`

*Source: [Why Companies Should Open Source and Host Their Own MCP Servers](https://lawrencewu.net/posts/2025-08-21-open-source-mcp-servers/)*

### GitHub Actions Integration

- Set up GitHub Actions with Claude Code to review PRs and generate commits/PRs
- Inspired by seeing the Anthropic team close an issue I'd opened by tagging `@claude can you fix it`

*Source: [Claude Code Agentic Coding Tips](https://lawrencewu.net/posts/2026-02-11-claude-code-agentic-coding/)*

### Other Engineering Work

- Creating and maintaining Cookiecutter templates for Python libraries
- Troubleshooting Kubernetes pods
- Writing documentation and Confluence pages via mcp-atlassian
- Creating presentations in ReactJS that are themed for the company, used the /frontend-slides skill to improve it

*Source: [Year in Review 2025](https://lawrencewu.net/posts/2025-12-31-year-in-review/)*

---

## Expanding Personal Projects

Uses outside of work that extend into personal productivity and creative output.

### Blog Post Visualizations & Writing

- Added graphs/visuals to blog posts (e.g., Long Beach Marathon data scraping and analysis)
- Used Claude Code + Claude Sonnet 4.5 to write the charitable contributions bunching article and generate code for visualizations
- Reviewed output and made edits, deleting ~75% of what was generated

*Source: [Bunching Charitable Contributions](https://lawrencewu.net/posts/2025-12-19-bunching-strategy/), [Year in Review 2025](https://lawrencewu.net/posts/2025-12-31-year-in-review/)*

### Annual Review Preparation (October 2025)

Used Claude Code to compile evidence of my own work:

- Fetched all commits from our private GitHub using `gh` CLI
- Pulled closed Jira tickets via Jira MCP
- Fetched all Confluence pages I'd authored via Confluence MCP
- Summarized work and matched it to stated goals

Result: "incredibly valuable in helping me write a rich annual review."

*Source: [Agentic Knowledge Work & Machine Learning](https://lawrencewu.net/posts/2026-03-04-agentic-knowledge-work/)*

---

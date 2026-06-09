# AI Portfolio Delivery System

AI-assisted portfolio delivery system documenting how Khang used **Open Design** and **Hermes** to ship and verify a live personal portfolio website.

Live site: https://www.im-khang.com/

GitHub proof repo: https://github.com/im-khang/ai-portfolio-delivery-system

## Business question

How can a personal portfolio website become credible proof of AI-assisted web/product delivery rather than a generic portfolio template?

## What this project demonstrates

This project demonstrates a practical agentic workflow:

- turning a vague personal-brand direction into a deployable website scope
- using **Open Design** as the website design/workbench layer
- using **Hermes** as an AI coding/operator agent for repo inspection, planning, file edits, QA, deployment checks, and documentation
- applying human review to keep claims honest, concise, and recruiter-readable
- verifying live site status before using the website as job-application proof

## Current verified deployment

- Canonical site: https://www.im-khang.com/
- Apex redirect: https://im-khang.com → https://www.im-khang.com/
- Verification date: 2026-06-09
- Verified status: `HTTP 200` on `https://www.im-khang.com/`
- Verified live-page markers: `Khang`, `Hermes`, `AI`, `portfolio`

Older deployment note:

- `https://01-agentic-portfolio-site.vercel.app/` returned Vercel `DEPLOYMENT_NOT_FOUND` during verification and is no longer the active public URL.

## Why Hermes matters here

Hermes was used as an AI coding/operator agent, not just a chat assistant.

Concrete agent work:

1. **Repo/deployment inspection**
   - checked local Git boundary
   - checked GitHub repo metadata
   - verified live domain response
   - detected stale/dead deployment URL

2. **Content strategy and claim control**
   - kept public copy tied to visible proof: live site, GitHub repos, command output, and application artifacts
   - flagged outdated deployment assumptions
   - kept unsupported backend/CMS/API/payment claims out of public proof

3. **Documentation and README patching**
   - rewrote the README around current verified deployment
   - documented Hermes/Open Design workflow proof
   - added prompt/QA receipts under `ai_agents/`
   - kept final case result under `reports/CASE_RESULT.md`

4. **Verification loop**
   - used HTTP status checks for live site and stale URL
   - fetched live HTML and checked markers
   - checked Git status before commit/push
   - verified final files before reporting completion

## Prompting / agent workflow receipts

See:

```text
ai_agents/prompts.md
ai_agents/workflow.md
ai_agents/qa_checklist.md
reports/CASE_RESULT.md
```

These files document how the project used Hermes prompting, Open Design workflow, QA checks, and human review.

## Featured proof links

- Live portfolio: https://www.im-khang.com/
- Agentic portfolio proof repo: https://github.com/im-khang/ai-portfolio-delivery-system
- Favorita Demand Planner Analytics: https://github.com/im-khang/favorita-demand-planner-analytics
- Olist Delivery SLA Risk Analytics: https://github.com/im-khang/olist-delivery-sla-risk-analytics

## Repository structure

```text
README.md
LICENSE
.gitignore
requirements.txt
data/
  raw/          # source/sample input files or local-only raw data
  interim/      # local-only transformed working files
  processed/    # local-only generated datasets
notebooks/      # ordered analysis notebooks/scripts
src/            # reusable project code
dashboard/      # BI/dashboard files or dashboard export code
docs/           # documentation and evaluation notes
reports/        # human-readable findings and figures
references/     # source notes, papers, dictionaries, original materials
scripts/        # verification or utility scripts
ai_agents/      # Hermes/Open Design workflow, prompts, QA evidence
```

## Setup

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

## Run / verify

```bash
python scripts/verify.py
```

## Public outputs

- Case result: `reports/CASE_RESULT.md`
- Evaluation notes: `docs/evaluation.md`
- Agent workflow: `ai_agents/workflow.md`
- Prompting receipts: `ai_agents/prompts.md`
- QA checklist: `ai_agents/qa_checklist.md`

## Data and security policy

- Credentials, environment files, local raw data, generated working data, databases, archives, and scratch outputs are ignored by `.gitignore`.
- Public repo keeps only shareable code, sample-safe artifacts, documentation, dashboard files, and evidence summaries.
- Claims should stay bounded by available data and documented assumptions.

## Claim boundary

This project proves:

- AI-assisted portfolio direction
- Open Design collaboration
- Hermes agentic coding/operator workflow
- human review and QA
- public deployment verification
- GitHub/Vercel/domain workflow awareness

This project does **not** claim:

- enterprise production automation
- backend platform engineering
- paid client delivery
- unsupported CMS/API/payment integrations
- AI-generated code shipped without human review

# Prompts and Hermes Usage Receipts

This file records the type of prompting and agent workflow used to develop, verify, and package the portfolio website proof.

## Operating prompt pattern

```text
Goal: turn current portfolio direction into a recruiter-facing web proof.
Constraints: preserve honest claims, keep project links real, avoid fake production claims, verify live deployment before reporting.
Deliverable: deployed site + GitHub README documenting AI-agent workflow and QA evidence.
```

## Prompt / task examples

### 1. Deployment verification

```text
Verify whether the portfolio site is live. Check current Vercel/domain URL, GitHub repo metadata, and live page markers. Do not assume old deployment URL still works.
```

Hermes action:

- inspected local repo remotes
- checked GitHub repo metadata with `gh`
- ran HTTP checks for old and current URLs
- found old `previous Vercel preview URL` deployment dead
- verified `https://www.im-khang.com/` is live

### 2. README proof documentation

```text
Document the live GitHub README showcasing my prompting and usage of Hermes as AI agent for coding my website as a proof.
```

Hermes action:

- rewrote README around current verified deployment
- documented Hermes as operator/agent layer
- documented Open Design as design/workbench layer
- added claim boundaries and verification evidence

### 3. Claim boundary review

```text
Make this useful for CDA Agentic Developer application, but do not overclaim backend/CMS/API production work if not proven.
```

Hermes action:

- framed portfolio as AI-assisted web/product delivery proof
- kept claim boundary explicit
- connected proof to real public URLs and GitHub repos

## Tools used by Hermes

- `git`: local repo boundary/status checks
- `gh`: GitHub repo metadata checks
- `curl`: live deployment status and HTML marker checks
- file patch/write tools: README and workflow documentation edits

## Human review points

- Whether portfolio claims sound like real work, not AI hype.
- Whether public project links are real and useful.
- Whether deployment is live before using it in an application.
- Whether README documents process clearly enough for a reviewer.

## Current verified public URL

```text
https://www.im-khang.com/
```

## Dead/stale URL found during verification

```text
the previous Vercel preview URL
```

Status observed: Vercel `DEPLOYMENT_NOT_FOUND`.

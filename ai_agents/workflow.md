# AI Agent Workflow

## Human goal

Build and ship a concise portfolio website for Khang that communicates practical-solution work, AI-assisted delivery, and human-reviewed project judgment.

## Agent-assisted workflow

1. Interpret positioning constraints and public claim boundaries.
2. Generate/refine visual direction through Open Design.
3. Use Hermes for repo inspection, content planning, file patching, QA, deployment verification, and documentation.
4. Apply human review to claims, tone, project naming, and public evidence.
5. Verify deployed domain behavior and live page markers after release.

## Hermes operator role

Hermes was used as an autonomous operator for the website proof, including:

- checking local Git repo boundary and dirty state
- checking GitHub repo metadata
- detecting stale deployment assumptions
- verifying live domain status with HTTP checks
- checking live HTML markers
- patching README and proof docs
- keeping claim boundaries explicit

## Human review points

- Portfolio wording says practical solutions, not generic website templates.
- Project proof uses real GitHub/live links.
- Public content does not expose private implementation notes.
- Claims stay tied to visible evidence: repo, command output, live URL, or verified file.
- Tone stays concise, recruiter-friendly, and honest.

## Verification used

- Public copy review.
- Stale wording review.
- Live route/domain check after deployment.
- Expected marker check on live page.
- GitHub repo metadata check.
- README/proof-document review.

## Result

Current active website:

```text
https://www.im-khang.com/
```

Dead/stale URL found:

```text
the previous Vercel preview URL
```

This proof repo documents the Hermes + Open Design workflow and current live deployment state.

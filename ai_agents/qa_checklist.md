# QA Checklist

## Public content

- [x] Direction says practical solutions, not generic website templates.
- [x] Project proof documents Hermes/Open Design workflow.
- [x] Public pages stay focused on project outcomes, not internal work notes.
- [x] Current live site URL is documented.
- [x] Stale/dead deployment URL is documented as inactive.
- [x] Contact/project proof links are present in README.

## Deployment verification

- [x] `https://www.im-khang.com/` returned HTTP `200` on 2026-06-09.
- [x] `https://im-khang.com` redirected to `https://www.im-khang.com/`.
- [x] Live HTML contained markers: `Khang`, `Hermes`, `AI`, `portfolio`.
- [x] Old `the previous Vercel preview URL` returned Vercel `DEPLOYMENT_NOT_FOUND` and should not be used as active URL.

## Repository hygiene

- [x] Repo keeps public proof/docs only.
- [x] README explains AI agent + Open Design workflow clearly.
- [x] Prompting/Hermes usage documented in `ai_agents/prompts.md`.
- [x] Workflow documented in `ai_agents/workflow.md`.
- [x] Case result documented in `reports/CASE_RESULT.md`.

## Human review

- [x] Claims stay tied to visible evidence.
- [x] No private local paths exposed in public content.
- [x] Claim boundary says no backend systems, paid client delivery, production automations, or enterprise integrations unless proven.

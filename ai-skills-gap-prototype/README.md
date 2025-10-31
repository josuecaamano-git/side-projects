# AI Skills Gap Prototype (WIP)

**Goal:** Help a job seeker understand the gap between their current profile and a target job description, then produce a targeted learning plan (skills, resources, sequence).

## What it does (concept)
- Input A: Candidate summary (e.g., CV highlights or LinkedIn About).
- Input B: Target role (job description text).
- Output:  
  - Skill match vs. gap (functional & technical).  
  - Priority gaps (Must-have vs. Nice-to-have).  
  - Action plan: courses, docs, hands-on mini-tasks.

## Current Status
- Early prototype. Prompts and mapping logic exist in draft form.  
- No production UI yet. Evaluating whether to build a simple web form or keep it CLI/notebook-based initially.

## Intended Users
- Job seekers targeting PM/PM-T roles.  
- Career coaches or bootcamps needing quick gap analyses.

## Approach (initial)
1. Parse JD text → extract required competencies (functional/technical).  
2. Parse candidate text → extract current competencies.  
3. Map to a normalized skill taxonomy (e.g., product, delivery, analytics, domain, tooling).  
4. Score and prioritize gaps.  
5. Generate a concise plan (what to learn, why, in what order).

## Example Output (sketch)
- **Strong:** Stakeholder management, Agile delivery, PRDs  
- **Gaps (high priority):** Authentication & identity fundamentals, threat models (basic), analytics instrumentation  
- **Plan (4 weeks):**  
  - Week 1: Identity basics (OAuth2/OIDC), SSO flows overview  
  - Week 2: Instrumentation: events, funnels, KPIs  
  - Week 3: Security and compliance basics for SaaS  
  - Week 4: Capstone—write a PRD for an auth-related feature

## Roadmap
- v0.1: Markdown report generator from two pasted texts (CV/JD).  
- v0.2: Simple web form (no auth, local run).  
- v0.3: Add curated learning links per gap (CH/EU-friendly when possible).  
- v0.4: Export to PDF.

## Risks / Limitations
- JD quality varies (may require manual cleanup).  
- Skill extraction accuracy depends on taxonomy coverage.

## Privacy
- No personal data stored by default. Inputs remain local unless explicitly saved by the user.

_Last updated: October 2025_

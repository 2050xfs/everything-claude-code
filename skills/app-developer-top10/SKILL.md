---
name: app-developer-top10
description: Top 10 essential skills every full-stack app developer (frontend + backend) should master, with references to deeper skill files in this repo.
origin: ECC
---

# Top 10 Skills for App Developers (Frontend + Backend)

A curated map of the most impactful skills for full-stack application developers.
Each entry links to a deeper skill file already in this repo where one exists.

## The List

### 1. Frontend Patterns
**Skill file:** `skills/frontend-patterns/SKILL.md`

Core React/Next.js patterns: component composition, state management (useState, useReducer, Zustand), data fetching (React Query, SWR, server components), performance optimization (memoization, code splitting, virtualization), and accessible UI design.

**Why it matters:** The user interface is the product. Poor component design compounds into slow, untestable UIs that are expensive to change.

---

### 2. Backend Patterns
**Skill file:** `skills/backend-patterns/SKILL.md`

RESTful and GraphQL API design, repository/service/controller layering, N+1 query prevention, Redis caching, rate limiting, background jobs, and middleware composition (auth, logging, validation).

**Why it matters:** Well-structured backends scale horizontally and stay maintainable as teams grow.

---

### 3. API Design
**Skill file:** `skills/api-design/SKILL.md`

Contract-first design, versioning strategies, consistent error shapes, pagination conventions, idempotency, and OpenAPI/GraphQL schema governance.

**Why it matters:** APIs are the contract between frontend and backend. Poorly designed APIs create cascading rework on both sides.

---

### 4. Database Migrations
**Skill file:** `skills/database-migrations/SKILL.md`

Safe, reversible schema changes; zero-downtime migration strategies (expand-contract pattern); index creation on live tables; backfill scripts; and migration testing in CI.

**Why it matters:** Schema changes are the riskiest deploys. A bad migration can bring down production for hours.

---

### 5. TDD Workflow
**Skill file:** `skills/tdd-workflow/SKILL.md`

Red-green-refactor cycle, test-first design for both unit and integration layers, mocking strategies, and using tests as living documentation.

**Why it matters:** Tests catch regressions, force better interfaces, and give developers the confidence to refactor aggressively.

---

### 6. E2E Testing
**Skill file:** `skills/e2e-testing/SKILL.md`

Browser automation with Playwright/Cypress, happy-path and critical-path coverage, flakiness prevention, visual regression testing, and CI integration.

**Why it matters:** Unit tests cannot catch integration failures between the UI, API, and database. E2E tests do.

---

### 7. Deployment Patterns
**Skill file:** `skills/deployment-patterns/SKILL.md`

CI/CD pipeline design, blue/green and canary releases, feature flags, environment promotion (dev → staging → prod), rollback procedures, and infrastructure-as-code basics.

**Why it matters:** Fast, reliable deploys are a competitive advantage. Slow or risky deploys slow down the entire team.

---

### 8. Docker Patterns
**Skill file:** `skills/docker-patterns/SKILL.md`

Multi-stage Dockerfiles, layer caching, local dev with Docker Compose (app + DB + cache), secrets management, health checks, and image size optimization.

**Why it matters:** Containers ensure environment parity from laptop to production and eliminate "works on my machine" problems.

---

### 9. Security Review
**Skill file:** `skills/security-review/SKILL.md`

OWASP Top 10 awareness, input validation and sanitization, SQL injection / XSS / CSRF prevention, secrets management (never commit credentials), dependency auditing, and auth/authz patterns (JWT, OAuth2, RBAC).

**Why it matters:** Security vulnerabilities are the highest-impact bugs. Most breaches exploit well-known, preventable flaws.

---

### 10. Design System
**Skill file:** `skills/design-system/SKILL.md`

Component libraries (shadcn/ui, Radix, Tailwind), design tokens (colors, spacing, typography), accessibility standards (WCAG 2.1 AA), responsive layout patterns, dark mode, and theming.

**Why it matters:** A shared design system cuts UI development time in half and ensures visual consistency across every screen.

---

## Quick-Reference Map

| # | Skill | Frontend | Backend | Skill File |
|---|-------|:--------:|:-------:|-----------|
| 1 | Frontend Patterns | ✓ | | `skills/frontend-patterns/` |
| 2 | Backend Patterns | | ✓ | `skills/backend-patterns/` |
| 3 | API Design | ✓ | ✓ | `skills/api-design/` |
| 4 | Database Migrations | | ✓ | `skills/database-migrations/` |
| 5 | TDD Workflow | ✓ | ✓ | `skills/tdd-workflow/` |
| 6 | E2E Testing | ✓ | ✓ | `skills/e2e-testing/` |
| 7 | Deployment Patterns | ✓ | ✓ | `skills/deployment-patterns/` |
| 8 | Docker Patterns | ✓ | ✓ | `skills/docker-patterns/` |
| 9 | Security Review | ✓ | ✓ | `skills/security-review/` |
| 10 | Design System | ✓ | | `skills/design-system/` |

## Learning Path Recommendation

**New developer** → Start with 1, 2, 3, then 10.
**Mid-level developer** → Add 5, 6, 9.
**Senior / tech lead** → Add 4, 7, 8.

## Related Skills Worth Exploring

- `skills/coding-standards/` — Language-agnostic style and quality baseline
- `skills/postgres-patterns/` — Deep SQL/Postgres optimization
- `skills/nextjs-turbopack/` — Next.js 15+ build tooling
- `skills/architecture-decision-records/` — Documenting technical decisions
- `skills/codebase-onboarding/` — Ramping up on an existing codebase quickly

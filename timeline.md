---
layout: default
title: Timeline
---

# Realistic Migration Timeline (2 Developers)
### Migration: Sanity → Contentful

> Assumes:
> - 2 full-time developers
> - 3–5 marketing-driven sites
> - Active production usage
> - No major redesign (pure CMS migration + refactor)

| Phase | Scope of Work | Key Activities | Est. Duration (2 Devs) | Notes / Risk Level |
|-------|--------------|----------------|------------------------|-------------------|
| **1. Executive Alignment & Planning** | Business + technical alignment | Confirm goals, audit current schemas, define migration scope, stakeholder buy-in | 1–2 weeks | Low risk but critical for clarity |
| **2. Content Model Redesign** | Rebuild Sanity schemas in Contentful | Map schema-as-code → UI models, define references, validations, environments | 2–3 weeks | Medium risk — modeling mistakes compound later |
| **3. Governance & Environment Setup** | Roles, permissions, workflows | Configure roles, staging/prod environments, publishing rules | 1–2 weeks | Medium — depends on org complexity |
| **4. Data Export & Transformation** | Sanity → Contentful format | Export dataset, write transformation scripts, handle references/assets | 2–3 weeks | High — relational integrity + edge cases |
| **5. Data Import & Validation** | Contentful Management API | Import entries, verify links, fix schema mismatches | 1–2 weeks | High — cleanup often required |
| **6. Frontend Refactor (API Layer)** | GROQ → GraphQL | Replace GROQ queries, rebuild data fetching, adjust caching | 2–4 weeks | High — touches many templates |
| **7. Preview & Editorial Workflow Rebuild** | Preview API + staging | Rebuild preview system, validate editor workflows | 1–2 weeks | Medium |
| **8. Multi-Site Architecture Setup** | Spaces / Environments | Configure brand separation strategy, test per-site queries | 1–2 weeks | Medium — depends on chosen structure |
| **9. QA & Regression Testing** | Full content + frontend audit | Content validation, SEO checks, preview verification | 2–3 weeks | High — production safety |
| **10. Editor Training & Cutover** | Change management | Documentation, training sessions, final content freeze + switch | 1–2 weeks | Medium — productivity dip likely |

---

# Total Estimated Timeline

| Scenario | Estimated Duration |
|----------|--------------------|
| **Optimistic (minimal complexity)** | 8–10 weeks |
| **Realistic (multi-site + active content)** | 10–14 weeks |
| **Complex (heavy personalization, many references)** | 14–18+ weeks |

---

# Parallel Work Considerations

With only 2 developers:

- Most phases cannot fully overlap.
- Frontend refactor cannot complete until content model stabilizes.
- Data import often reveals modeling issues requiring iteration.
- Marketing output may slow during weeks 4–10.

---

# Key Timeline Drivers

| Driver | Impact |
|--------|--------|
| Number of content types | Directly increases modeling time |
| Nested references | Increases data migration complexity |
| Personalization metadata | Impacts schema + frontend |
| Multi-site structure | Adds environment & query complexity |
| Editor count | Increases training & QA time |

---

# Executive Interpretation

For a 2-developer team:

- Migration is **not a light refactor** — it is a multi-month platform transition.
- The bulk of effort sits in **content modeling + frontend refactoring**.
- Risk is highest during **data migration and QA phases**.
- Opportunity cost includes slowed feature velocity during migration.

---

If you'd like, I can also create:
- A cost-adjusted timeline with estimated developer hours
- A side-by-side "Stay on Sanity vs Migrate" effort comparison
- Or a visual Gantt-style breakdown

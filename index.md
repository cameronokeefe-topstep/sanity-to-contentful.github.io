---
layout: default
title: Overview
active: true
---

# Core Positioning Differences

## Sanity (Composable Content Cloud)

Best when you want maximum flexibility and speed through engineering leverage.

- **Schema as code**: Content types are defined in code and versioned like software (PRs, CI/CD). Ideal when your site and content model evolve quickly and you want changes to be reviewable, testable, and repeatable.
- **Real-time collaboration**: Strong live editing and collaborative workflows, especially valuable for distributed teams.
- **Content Lake concept**: Centralized content backend designed to power multiple frontends and channels.
- **Modern frontend alignment**: Typically shines with a Next.js / modern frontend team ready to build a tailored authoring experience.

---

## Contentful (Composable Content Platform / DXP Direction)

Best when you want marketing-friendly scale and governance, often within a more enterprise operating model.

- **Composable platform story**: Structured, reusable content designed for multi-channel delivery.
- **Marketer-facing experience tooling**: Expanding into low-code / experience-building capabilities alongside the core platform.
- **Enterprise controls + ecosystem**: Strong out-of-the-box governance and broad integration marketplace.
- **Platform-led approach**: Fits teams that prefer operating within established conventions rather than deeply customizing the CMS UI.

---

# Sanity vs Contentful — Key Features, Benefits, Drawbacks

| Category | Sanity | Contentful |
|-----------|----------|-------------|
| **Core Positioning** | Composable Content Cloud focused on flexibility and developer control | Composable Content Platform with enterprise governance and DXP direction |
| **Content Modeling** | **Feature:** Schema-as-code (defined in JavaScript/TypeScript) <br> **Benefits:** Full control, versioned via Git, highly adaptable <br> **Drawbacks:** Requires developer involvement for structural changes | **Feature:** UI-driven content model builder <br> **Benefits:** Easier for non-devs to adjust models <br> **Drawbacks:** Less flexible, constrained by platform patterns |
| **Editor Experience** | **Feature:** Fully customizable Studio (open-source) <br> **Benefits:** Can tailor workflows, previews, inputs to match marketing needs <br> **Drawbacks:** Requires setup effort to optimize UX | **Feature:** Guided, structured editorial UI <br> **Benefits:** Lower cognitive load, standardized experience <br> **Drawbacks:** Deep customization limited without engineering |
| **Landing Page Building** | **Feature:** Composable modular sections system (custom-built) <br> **Benefits:** Extremely flexible once implemented <br> **Drawbacks:** Requires upfront development investment | **Feature:** Experience Builder / marketplace tools <br> **Benefits:** Faster marketer autonomy early on <br> **Drawbacks:** Less freedom outside provided UI paradigms |
| **Real-Time Collaboration** | **Feature:** Live editing + real-time presence <br> **Benefits:** Excellent for distributed teams <br> **Drawbacks:** None significant at mid-size scale | **Feature:** Collaborative editing <br> **Benefits:** Stable, structured collaboration <br> **Drawbacks:** Not as deeply real-time oriented as Sanity |
| **Governance & Roles** | **Feature:** Role-based permissions (configurable) <br> **Benefits:** Flexible if engineered properly <br> **Drawbacks:** Governance structure often requires customization | **Feature:** Enterprise-grade roles, environments, approvals <br> **Benefits:** Strong out-of-the-box governance <br> **Drawbacks:** Operates within platform conventions |
| **APIs & Querying** | **Feature:** GROQ query language + APIs <br> **Benefits:** Extremely flexible querying <br> **Drawbacks:** Learning curve for teams unfamiliar with GROQ | **Feature:** REST + GraphQL APIs <br> **Benefits:** Familiar to many developers <br> **Drawbacks:** Less expressive than GROQ for complex querying |
| **Personalization Readiness** | **Feature:** Fully customizable schemas + webhooks <br> **Benefits:** Easy to model experiment variants and metadata <br> **Drawbacks:** Personalization logic lives outside CMS | **Feature:** Strong ecosystem integrations <br> **Benefits:** Marketplace integrations for experimentation stacks <br> **Drawbacks:** Still requires external personalization tooling |
| **Integrations & Ecosystem** | **Feature:** Growing ecosystem + webhooks <br> **Benefits:** Flexible integration via APIs <br> **Drawbacks:** Fewer turnkey integrations | **Feature:** Large marketplace + enterprise integrations <br> **Benefits:** Broader plug-and-play ecosystem <br> **Drawbacks:** May increase platform dependency |
| **Frontend Alignment** | **Feature:** Designed for modern stacks (Next.js, React, Vercel) <br> **Benefits:** Excellent fit for product-led web teams <br> **Drawbacks:** Assumes engineering maturity | **Feature:** Framework-agnostic APIs <br> **Benefits:** Works across stacks <br> **Drawbacks:** Less tightly aligned with frontend-as-product mindset |
| **Scalability** | **Feature:** Central Content Lake architecture <br> **Benefits:** Multi-channel, multi-site ready <br> **Drawbacks:** Governance scaling requires planning | **Feature:** Enterprise platform scaling <br> **Benefits:** Strong multi-brand, multi-region support <br> **Drawbacks:** Higher cost at scale |
| **Cost Structure** | **Benefit:** Lower per-seat cost (growth tiers affordable) <br> **Drawback:** Developer time is primary investment | **Benefit:** Enterprise features bundled in higher tiers <br> **Drawback:** Seats + API usage can become expensive |
| **Best Fit Scenario** | Teams with strong frontend developers who want maximum flexibility and custom workflows | Organizations prioritizing standardized governance, enterprise controls, and lower initial customization |

---

## Quick Summary

- **Choose Sanity** if flexibility, modular content architecture, and developer-driven velocity are top priorities.
- **Choose Contentful** if enterprise governance, standardized workflows, and broader out-of-the-box integrations are the primary drivers.

---

# Landing Page Velocity (What Marketing Feels Most)

## Where Sanity Tends to Win

- **Fast iteration after setup**: Once a modular “sections” system (hero, testimonials, FAQ, CTA, etc.) is built, marketing can assemble pages quickly.
- **Engineering extensibility**: Developers can add new modules without being constrained by rigid UI patterns.
- **Excellent preview workflows**: Real-time editing paired with frontend preview tooling (common in Next.js/Vercel setups).

**Tradeoff:** Requires upfront investment to design and build the authoring experience marketing wants.

---

## Where Contentful Tends to Win

- **Earlier marketer autonomy**: Faster time to usable page-building capabilities with less custom CMS development.
- **Governance-aligned velocity**: Easier to roll out structured approval workflows in organizations with compliance, legal, or brand review requirements.
- **Lower initial customization lift**: Less need to deeply configure the editorial UI before marketing can start shipping pages.

---

# Governance, Approvals, Roles (Brand Safety at Speed)

## Sanity

- Governance is highly configurable but often depends on how Studio is implemented.
- Best when marketing and web teams collaborate closely.
- Works well if you are comfortable treating content structure as product surface area managed via code.

## Contentful

- Often preferred when standardized governance patterns are required across teams and regions.
- Clearer enterprise permission models out of the box.
- Strong fit when you want predictable, platform-defined workflows.

---

# Personalization / Experimentation Readiness (Growth Loops)

## Sanity

- Strong when personalization lives in the frontend or experimentation platform (Optimizely, LaunchDarkly, homegrown rules).
- Developers can easily model experiment variants, audience rules, and reusable content blocks.
- Well-suited to product-led growth environments.

## Contentful

- Investing heavily in DXP-style capabilities, including AI and personalization directions.
- Frequently integrated into enterprise experimentation stacks.
- Good fit when experimentation is coordinated across multiple teams and sys




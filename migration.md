---
layout: default
title: Migration
---

# Migration Overview: Sanity → Contentful

> Key Vendor References  
> - <a href="https://www.sanity.io/docs" target="_blank" rel="noopener noreferrer">Sanity Documentation</a>  
> - <a href="https://www.sanity.io/docs/groq" target="_blank" rel="noopener noreferrer">Sanity GROQ</a>  
> - <a href="https://www.sanity.io/docs/exporting-data" target="_blank" rel="noopener noreferrer">Sanity Data Export</a>  
> - <a href="https://www.contentful.com/developers/docs/" target="_blank" rel="noopener noreferrer">Contentful Developer Documentation</a>  
> - <a href="https://www.contentful.com/developers/docs/references/graphql/" target="_blank" rel="noopener noreferrer">Contentful GraphQL API</a>  
> - <a href="https://www.contentful.com/developers/docs/concepts/data-model/" target="_blank" rel="noopener noreferrer">Contentful Content Modeling Guide</a>  
> - <a href="https://www.contentful.com/help/roles-and-permissions/" target="_blank" rel="noopener noreferrer">Contentful Roles & Permissions</a>  
> - <a href="https://www.contentful.com/developers/docs/concepts/multiple-environments/" target="_blank" rel="noopener noreferrer">Contentful Environments</a>  

---

# 1. Executive Summary

This section defines the business rationale for migration and clarifies what the organization expects to gain. It ensures stakeholders are aligned on goals such as editorial autonomy, governance improvements, scalability, and long-term platform strategy before technical work begins.

## Purpose of Migration
- Improve editorial autonomy  
- Reduce developer dependency  
- Standardize content modeling across teams  
  (<a href="https://www.contentful.com/developers/docs/concepts/data-model/" target="_blank" rel="noopener noreferrer">Content Modeling Guide</a>)  
- Enable stronger enterprise governance  
  (<a href="https://www.contentful.com/help/roles-and-permissions/" target="_blank" rel="noopener noreferrer">Roles & Permissions</a>)  

---

# 2. Strategic Considerations

This section evaluates how the CMS decision supports broader business objectives. It connects platform capabilities to marketing speed, multi-brand management, compliance requirements, and long-term operational scale.

- Marketing velocity  
  <a href="https://www.contentful.com/solutions/marketing/" target="_blank" rel="noopener noreferrer">Marketing Solutions</a>  
- Multi-site management  
  <a href="https://www.contentful.com/developers/docs/concepts/multiple-environments/" target="_blank" rel="noopener noreferrer">Multiple Environments</a>  
- Governance & compliance  
  <a href="https://www.contentful.com/help/roles-and-permissions/" target="_blank" rel="noopener noreferrer">Roles & Permissions</a>  

---

# 3. Technical Considerations

This section outlines the engineering impact of migration. It is critical for estimating timeline, complexity, and resource allocation, including schema redesign, API transitions, validation rebuilding, and frontend refactoring.

- Replace GROQ  
  <a href="https://www.sanity.io/docs/groq" target="_blank" rel="noopener noreferrer">GROQ</a>  
  with GraphQL  
  <a href="https://www.contentful.com/developers/docs/references/graphql/" target="_blank" rel="noopener noreferrer">GraphQL API</a>  
- Rebuild schemas  
  <a href="https://www.contentful.com/developers/docs/concepts/data-model/" target="_blank" rel="noopener noreferrer">Content Modeling</a>  
- Recreate validations  
  <a href="https://www.contentful.com/developers/docs/concepts/validations/" target="_blank" rel="noopener noreferrer">Validations</a>  

---

# 4. Editorial Experience Comparison

This section compares how each platform supports content authors. Editorial usability directly affects marketing productivity, onboarding time, and long-term content governance consistency.

**Sanity**
- <a href="https://www.sanity.io/docs/studio" target="_blank" rel="noopener noreferrer">Customizable Studio</a>  
- <a href="https://www.sanity.io/docs/schema-types" target="_blank" rel="noopener noreferrer">Schema-as-code</a>  

**Contentful**
- <a href="https://www.contentful.com/developers/docs/concepts/data-model/" target="_blank" rel="noopener noreferrer">Structured Modeling</a>  
- <a href="https://www.contentful.com/developers/docs/concepts/editor-interfaces/" target="_blank" rel="noopener noreferrer">Editor Interfaces</a>  

---

# 5. Governance & Enterprise Controls

This section addresses risk management and operational maturity. For organizations with compliance requirements, multiple teams, or staged release workflows, governance capabilities are often a deciding factor.

- <a href="https://www.contentful.com/help/roles-and-permissions/" target="_blank" rel="noopener noreferrer">Roles & Permissions</a>  
- <a href="https://www.contentful.com/developers/docs/concepts/multiple-environments/" target="_blank" rel="noopener noreferrer">Environments</a>  
- <a href="https://www.contentful.com/enterprise/" target="_blank" rel="noopener noreferrer">Enterprise Offering</a>  

---

# 6. Data Migration Plan

This section defines how existing content will be exported, transformed, and imported. It is essential for protecting data integrity, preserving relationships between entries, and minimizing disruption during cutover.

- Export data  
  <a href="https://www.sanity.io/docs/exporting-data" target="_blank" rel="noopener noreferrer">Sanity Export</a>  
- Import via  
  <a href="https://www.contentful.com/developers/docs/references/content-management-api/" target="_blank" rel="noopener noreferrer">Content Management API</a>  

---

# 7. Frontend & API Changes

This section highlights application-level changes required to consume Contentful APIs. It impacts performance, caching strategies, preview workflows, and developer maintenance patterns.

- GraphQL usage  
  <a href="https://www.contentful.com/developers/docs/references/graphql/" target="_blank" rel="noopener noreferrer">GraphQL API</a>  
- Preview API  
  <a href="https://www.contentful.com/developers/docs/references/content-preview-api/" target="_blank" rel="noopener noreferrer">Preview API</a>  

---

# 8. Cost & Licensing

This section evaluates financial implications beyond subscription fees, including API metering, seat-based pricing, and long-term total cost of ownership compared to maintaining a customized Sanity implementation.

- Pricing  
  <a href="https://www.contentful.com/pricing/" target="_blank" rel="noopener noreferrer">Pricing</a>  
- Delivery API limits  
  <a href="https://www.contentful.com/developers/docs/references/content-delivery-api/" target="_blank" rel="noopener noreferrer">Content Delivery API</a>  

---

# 9. Risks & Tradeoffs

This section identifies potential downsides of migration, including reduced schema flexibility, vendor lock-in, and possible scaling costs. Understanding tradeoffs helps prevent unintended architectural constraints.

- Loss of schema-as-code  
  <a href="https://www.sanity.io/docs/schema-types" target="_blank" rel="noopener noreferrer">Schema Types</a>  
- API rate limits  
  <a href="https://www.contentful.com/developers/docs/references/content-delivery-api/" target="_blank" rel="noopener noreferrer">Content Delivery API</a>  

  ### Schema-as-Code (Deep Dive)

    Schema-as-code means your CMS content model is defined in code (JavaScript/TypeScript), versioned in Git, and deployed like application logic — instead of being configured only through a web UI.

    This approach treats your content structure as part of your product architecture, not just CMS configuration.
    

    ### What Schema-as-Code Actually Looks Like

    In a schema-as-code system (like Sanity), you define content types programmatically:

    ```ts
    export default {
      name: 'landingPage',
      type: 'document',
      fields: [
        { name: 'title', type: 'string', validation: Rule => Rule.required() },
        { name: 'slug', type: 'slug' },
        { name: 'sections', type: 'array', of: [{ type: 'hero' }, { type: 'faq' }] }
      ]
    }
    ```

---

# 10. Decision Framework & Recommendation

This section provides structured criteria for leadership to evaluate whether migration aligns with organizational priorities. It ensures the decision is based on long-term strategy rather than short-term feature comparisons.

- Governance priority → Contentful  
  <a href="https://www.contentful.com/help/roles-and-permissions/" target="_blank" rel="noopener noreferrer">Roles & Permissions</a>  
- Flexibility priority → Sanity  
  <a href="https://www.sanity.io/docs/schema-types" target="_blank" rel="noopener noreferrer">Schema Types</a>  
- Compare total cost  
  <a href="https://www.contentful.com/pricing/" target="_blank" rel="noopener noreferrer">Pricing</a>  

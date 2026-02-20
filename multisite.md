---
layout: default
title: Multisite
---

# 🌐 Multi-Site in Sanity

Sanity is extremely well suited for multi-brand architecture because of its flexible data modeling and centralized content backend.

---

## 1️⃣ Single Dataset, Multi-Site Model

With a single dataset, you can support multiple brands cleanly by modeling site context into your content.

You can:

- Add a `site` field to content documents  
- Use site-specific document types  
- Scope queries per site  
- Share components across brands  
- Separate themes in the frontend  

This allows you to manage:

- Shared blog content  
- Brand-specific landing pages  
- Shared product data  
- Separate SEO configurations  

All inside one Studio.

This approach keeps operations centralized while allowing content and presentation to vary per brand.

---

## 2️⃣ Multiple Datasets (If Needed)

If stronger separation is required, Sanity supports multiple datasets.

You can:

- Create one dataset per brand  
- Use one Studio to manage multiple datasets  
- Share schemas across brands  
- Maintain separate publishing environments  

This provides isolation where necessary while keeping development and governance centralized.

---

## 3️⃣ Flexible Theming

Because your frontend controls presentation:

- You can use the same content model across brands  
- Apply different styling layers per brand  
- Reuse layout components  
- Reduce developer duplication  

Sanity’s structured content approach makes cross-brand reuse clean and efficient, especially for teams using modern frontend frameworks like Next.js.

---

## Why This Matters

Sanity allows you to scale multi-site architecture without forcing structural duplication.  
You control whether separation happens at the content layer (dataset) or presentation layer (frontend), giving you architectural flexibility as your brand portfolio grows.

---

# 🌐 Multi-Site in Contentful

Contentful supports multi-site architectures through:

- **Spaces** (often one per brand)
- **Environments** (dev, staging, production)
- **Shared content models**
- **Role-based permissions**

This structure works well when governance and brand separation are top priorities.

---

## ⚠ Operational Considerations

When using separate Spaces per brand, you may encounter:

- Content duplication across brands  
- Sync overhead between shared content  
- Higher pricing tiers as spaces, seats, and API usage increase  
- More operational complexity managing permissions and deployments  

---

## Where Contentful Shines

For enterprise organizations with:

- Dozens of brands  
- Regional or global content teams  
- Strict compliance and governance requirements  

Contentful’s structured separation model can provide clarity and control at scale.

---

## For 4 Marketing-Driven Sites with 2 Developers?

It may introduce more complexity than necessary.  
Operational overhead and migration cost could outweigh governance benefits.

---

# 🛠 Realistic Engineering Comparison

| Factor | Stay on Sanity | Move to Contentful |
|---------|----------------|-------------------|
| **Migration Time** | 0 | 8–14 weeks |
| **Multi-Site Setup** | 2–4 weeks | 10–14+ weeks (including migration) |
| **Developer Control** | High | Moderate |
| **Cost Scaling** | Predictable | Likely higher |
| **Marketing Flexibility** | High | High, but more constrained |
| **Risk Level** | Low | Medium–High |
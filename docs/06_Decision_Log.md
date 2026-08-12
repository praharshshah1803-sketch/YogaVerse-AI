# Decision Log

## DEC-001: Supabase over Firebase
**Date:** 2026-08-12  
**Decision:** Use Supabase for the initial backend.  
**Alternatives:** Firebase; custom Node.js + PostgreSQL.  
**Reasoning:** PostgreSQL gives us a strong relational foundation and native pgvector support for a later RAG layer. Supabase also provides authentication, row-level security, storage, and edge functions without maintaining a separate backend stack during the pilot.  
**Tradeoff:** The team will have a smaller ecosystem of opinionated examples than Firebase.  
**Revisit if:** Database/vector workloads or operational requirements justify a dedicated backend.

## DEC-002: RAG over fine-tuning for the wellness coach
**Date:** 2026-08-12  
**Decision:** Ground the assistant in approved Yoga By Rachna Shah knowledge using retrieval rather than fine-tuning in the MVP.  
**Reasoning:** The knowledge base will evolve and needs traceability and easy content updates. RAG makes it easier to remove outdated content and show source context.  
**Tradeoff:** Retrieval quality becomes a critical dependency.  
**Revisit if:** Stable tone or behavior cannot be achieved through prompt + retrieval controls.

## DEC-003: OpenAI API as initial LLM
**Date:** 2026-08-12  
**Decision:** Start with OpenAI for the MVP and establish a model-comparison harness before locking the model long term.  
**Reasoning:** Fastest route to prototyping, strong structured-output capabilities, and broad tooling support.  
**Tradeoff:** Vendor cost and dependency.  
**Revisit if:** Another model materially improves quality, latency, or unit economics on the same evaluation set.

## DEC-004: Next.js over plain React
**Date:** 2026-08-12  
**Decision:** Use Next.js for the eventual application frontend.  
**Reasoning:** The product has public landing pages that benefit from SEO and authenticated application screens that can use the same codebase.  
**Tradeoff:** More framework conventions than a simple client-rendered React app.  
**Revisit if:** The product becomes primarily a static client application.

## DEC-005: PostHog over Mixpanel / Amplitude
**Date:** 2026-08-12  
**Decision:** Use PostHog for initial product analytics.  
**Reasoning:** We need event funnels, retention views, and experimentation with a relatively small engineering footprint.  
**Tradeoff:** The team will need to define a clean event taxonomy early to avoid noisy analytics.  
**Revisit if:** Scale or governance requirements make another analytics platform materially better.

## DEC-006: pgvector over Pinecone for the first RAG implementation
**Date:** 2026-08-12  
**Decision:** Keep vectors close to the operational database initially.  
**Reasoning:** Fewer moving parts and simpler synchronization for a pilot.  
**Tradeoff:** Dedicated vector infrastructure may become preferable at larger scale.  
**Revisit if:** Retrieval performance or index scale becomes a bottleneck.

## DEC-007: Yoga By Rachna Shah as the first pilot
**Date:** 2026-08-12  
**Decision:** Validate with the existing brand before opening the platform to multiple businesses.  
**Reasoning:** A real operator provides faster feedback on instructor workflows, content quality, and conversion than a hypothetical multi-tenant launch.  
**Tradeoff:** Some early product decisions may be specific to this brand and require abstraction later.  
**Revisit if:** Pilot learning is strong enough to justify multi-brand architecture work.

## DEC-008: Wellness guidance, not medical diagnosis
**Date:** 2026-08-12  
**Decision:** Position AI output as general wellness guidance and route medical questions to appropriate professionals.  
**Reasoning:** This reduces user-risk and keeps the product aligned with the role of a yoga/wellness platform.  
**Tradeoff:** The assistant will intentionally refuse or redirect some requests.  
**Revisit if:** Regulatory and clinical capabilities materially change in a future product version.

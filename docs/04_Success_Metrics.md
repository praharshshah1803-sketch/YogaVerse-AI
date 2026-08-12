# Success Metrics & KPI Framework

## North Star Metric
**Weekly Active Practitioners (WAP):** unique students who complete at least one AI-recommended yoga/wellness session in a calendar week.

The North Star is intentionally behavior-based. An assessment alone is not value; the product should help a user take an appropriate next step.

## Input metrics

| Metric | Definition | Baseline | 30-day target | 90-day target | Measurement | Owner |
|---|---|---:|---:|---:|---|---|
| Assessment completion rate | Started assessments that reach a submitted profile | 0% pre-launch | 60% | 70% | PostHog event funnel | Product |
| Recommendation CTR | Users clicking at least one recommended program/instructor | 0% | 45% | 55% | PostHog | Product |
| Instructor profile completion | Approved instructors completing required profile fields | 0% | 80% | 90% | Supabase + PostHog | Admin |

## Output metrics

| Metric | Definition | Baseline | 30-day target | 90-day target | Measurement | Owner |
|---|---|---:|---:|---:|---|---|
| Paid conversion rate | Eligible users who purchase a paid offering after assessment | 0% | 8% | 15% | Checkout + PostHog | Business |
| Monthly recurring revenue | Revenue from active subscription plans in a month | ₹0 | ₹25k | ₹1L | Payment system | Business |
| 30-day retention | Users active in week 1 who return and complete a session around day 30 | 0% | 20% | 30% | Cohort analysis | Product |
| 60-day retention | Users active in week 1 who return around day 60 | 0% | 12% | 20% | Cohort analysis | Product |
| 90-day retention | Users active in week 1 who return around day 90 | 0% | 8% | 15% | Cohort analysis | Product |

## AI-specific metrics

| Metric | Definition | Baseline | 30-day target | 90-day target | Measurement | Owner |
|---|---|---:|---:|---:|---|---|
| Recommendation acceptance | Recommended path started or selected by user | 0% | 50% | 60% | Product event | AI/Product |
| AI response quality | Average human/user rating on usefulness, relevance and tone | N/A | 4.0/5 | 4.2/5 | In-product survey + human eval | AI/Product |
| Hallucination rate | Evaluated outputs containing unsupported factual claims | N/A | <7% | <5% | Curated eval set | AI/Product |
| Instructor match satisfaction | Users rating recommended instructor 4/5+ | N/A | 55% | 65% | Post-match survey | Product |

## Guardrail / health metrics

| Metric | Definition | Baseline | 30-day target | 90-day target | Measurement | Owner |
|---|---|---:|---:|---:|---|---|
| AI response time | P95 time to first complete response | N/A | <6 sec | <4 sec | Application telemetry | Engineering |
| Harmful-content rate | Safety-critical outputs in audited sample | N/A | 0% | 0% | AI safety evaluation | Product/AI |
| Student NPS | Likelihood to recommend YogaVerse AI | N/A | +20 | +35 | Monthly survey | Business |
| Instructor churn | Active instructors leaving platform during period | N/A | <8% monthly | <5% monthly | Subscription/admin records | Business |

## Measurement principles

- Targets above are **pilot targets**, not claims about the current business.
- Baselines must be replaced with observed values once instrumentation is live.
- Metrics should be segmented by user type, acquisition source, program type, and instructor where sample size permits.
- Safety metrics can override growth goals; a conversion lift is not considered positive if it comes from unsafe or misleading AI guidance.

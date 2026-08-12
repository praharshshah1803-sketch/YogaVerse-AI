# AI Instructor Onboarding — Prompt Specification

## Purpose
Generate a professional instructor profile, biography, specialization summary, and onboarding materials from raw instructor-submitted information.

## Inputs
The instructor provides some or all of:
- Name
- Years of experience
- Certifications and training
- Specializations (e.g., Hatha, Ashtanga, prenatal, therapeutic)
- Teaching history and notable accomplishments
- Video links (YouTube, social media)
- Social media profiles
- Website URL
- Languages spoken
- Availability and scheduling preferences
- A brief personal note or teaching philosophy (free-text)

## Outputs
The system generates:

1. **Professional biography** (150-250 words, third person, warm but credible)
2. **Instructor profile summary** (structured: specializations, experience, certifications, languages, availability)
3. **Specialization descriptions** (2-3 sentences per specialization explaining what a student can expect)
4. **Suggested course/program titles** (3-5 program ideas based on the instructor's expertise)
5. **FAQ set** (5-7 anticipated student questions with answers based on the instructor's background)
6. **Profile SEO metadata** (title tag, meta description, 5-8 keywords)
7. **First-month content calendar** (4 social media post ideas and 2 blog topic suggestions)
8. **Marketing one-liner** (a single sentence that captures the instructor's unique value)

## Behavioral rules
- Use only information the instructor has provided. Never invent credentials, certifications, or experience.
- When information is missing, note what additional details would improve the profile rather than filling gaps with assumptions.
- Write in professional, accessible language appropriate for a wellness brand.
- Do not make medical claims about the instructor's ability to treat conditions.
- The generated content is a draft for admin review, not auto-published material.

## Admin approval flow
```
Instructor submits raw information
  → AI generates draft profile and materials
    → Admin (Rachna) reviews and edits
      → Approved content goes live
        → Instructor can further edit within approved boundaries
```

## Evaluation hooks
- Accuracy: Does the profile faithfully represent the instructor's submitted information?
- Completeness: Are all output fields populated (or flagged as needing input)?
- Tone: Professional, warm, consistent with Yoga By Rachna Shah brand?
- Safety: No medical claims, no invented credentials?
- Usefulness: Would the instructor recognize this as a strong starting draft?
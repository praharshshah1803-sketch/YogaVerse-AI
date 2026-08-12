# YogaVerse AI

> An AI-powered operating system for yoga and wellness businesses.

## Why this project exists

YogaVerse AI is a product experiment built around **Yoga By Rachna Shah**, an existing yoga and wellness business. The goal is to understand whether AI can improve two sides of the business at the same time:

- **Students:** help people discover an appropriate yoga journey instead of navigating a large library of generic content.
- **Instructors and business operators:** reduce repetitive work, improve digital presence, and make it easier to scale the brand through trusted instructors.

This is being developed as a real-world AI Product Management case study, not as a generic chatbot demo.

## Product thesis

The initial product loop is:

**Discover → Assess → Personalize → Recommend → Convert**

The longer-term platform adds AI instructor onboarding, subscriptions, a RAG-powered wellness coach, content automation, analytics, and eventually multi-brand capabilities.

## Phase 1 scope

The first release focuses on proving the student-facing journey while keeping the architecture ready for instructor workflows.

- [x] Product vision
- [x] Problem hypotheses
- [x] User personas
- [x] KPI framework
- [x] Prioritized feature backlog
- [x] Decision log
- [x] AI evaluation framework
- [x] Hypothesis tracker
- [x] Responsible AI framework
- [x] Competitive-analysis framework
- [ ] User interviews
- [ ] Phase 1 PRD
- [ ] User flows and wireframes
- [ ] High-fidelity UI
- [ ] Working AI assessment MVP
- [ ] Analytics instrumentation

## Planned product capabilities

### Student
- AI wellness assessment
- Personalized starting plan
- Instructor recommendation
- Instructor profiles
- Consultation / booking CTA
- Later: RAG wellness coach, progress tracking, subscriptions

### Instructor
- AI-assisted onboarding
- Profile generation
- Course/program creation
- Content studio
- Student and business analytics

### Business owner / admin
- Instructor approval
- Brand and content governance
- Lead and conversion analytics
- Subscription and revenue visibility

## AI architecture direction

**Frontend:** React / Next.js  
**Backend:** Supabase + PostgreSQL  
**AI:** OpenAI API initially, with model comparison later  
**RAG:** pgvector + approved Yoga By Rachna Shah knowledge  
**Automation:** n8n  
**Analytics:** PostHog  
**Design:** Figma

The repository deliberately separates product documentation, research, prompts, AI evaluation, design, frontend, and backend work so the build remains auditable and easy to discuss in an interview.

## Product principles

1. Wellness guidance, never medical diagnosis.
2. AI amplifies the instructor; it does not replace human judgment.
3. Use brand-specific knowledge instead of generic answers wherever possible.
4. Validate assumptions with users before scaling the platform.
5. Treat safety and trust as product metrics, not compliance afterthoughts.

## Repository map

| Folder | Purpose |
|---|---|
| `docs/` | Product strategy, personas, metrics, decisions, AI evaluation, hypotheses, responsible AI |
| `research/` | Competitor research, interview materials, market research |
| `design/` | Wireframes, flows, information architecture |
| `prd/` | Product requirement documents |
| `prompts/` | Reusable AI prompt specifications |
| `ai/` | Evaluation and RAG architecture |
| `frontend/` | Application UI |
| `backend/` | Backend and data layer |
| `assets/` | Brand and product assets |

## Current status

**Stage:** Day 1 — Product Foundation  
**Pilot:** Yoga By Rachna Shah  
**Primary PM question:** Can a personalized, AI-assisted discovery journey improve the first-time student's path to a relevant yoga program or instructor while creating a scalable operating model for the business?

## Portfolio context

This repository is intended to demonstrate practical AI Product Management skills across discovery, strategy, experimentation, AI evaluation, UX, engineering collaboration, analytics, and business model design.

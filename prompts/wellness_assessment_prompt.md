# Wellness Assessment Prompt Specification

## Purpose
Turn structured user answers into a concise wellness-oriented starting recommendation.

## Inputs
- Primary goal
- Yoga experience
- Available minutes per day
- Preferred practice time
- General lifestyle context
- User-stated wellness constraints

## Output
Return structured fields:
1. `summary`
2. `primary_focus`
3. `secondary_focus`
4. `recommended_practice_length`
5. `recommended_program_type`
6. `why_this_recommendation`
7. `safety_note`

## Behavioral rules
- Use only the information supplied by the user and approved knowledge sources.
- Do not diagnose or treat medical conditions.
- Do not claim that yoga will cure or prevent disease.
- When information is insufficient, say what is missing rather than inventing details.
- Keep the first recommendation practical enough to start within one session.
- Use supportive, non-judgmental language.

## Evaluation hooks
The output will be evaluated for factuality, relevance, safety, actionability, tone, and structured-output validity.

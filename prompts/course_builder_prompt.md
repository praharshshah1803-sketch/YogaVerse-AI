# AI Course Builder — Prompt Specification

## Purpose
Transform raw instructor materials into a structured course with modules, lessons, descriptions, and marketing copy.

## Inputs
The instructor provides one or more of:
- PDF documents (lesson plans, handouts)
- Written notes or outlines
- Voice note transcripts
- Existing video links with descriptions
- A rough course outline or topic list
- Target audience description
- Course duration preference

## Outputs

1. **Course structure**
   - Course title and subtitle
   - Course description (150-200 words)
   - Target audience statement
   - Prerequisites (if any)
   - Expected outcomes (3-5 bullet points)

2. **Module breakdown**
   - Module title
   - Module description (2-3 sentences)
   - Estimated duration
   - Key learning objectives

3. **Lesson outlines** (per module)
   - Lesson title
   - Lesson summary
   - Key poses/practices covered
   - Suggested homework or self-practice

4. **Course FAQ** (5-8 questions)
   - Anticipated student questions with answers

5. **Landing page copy**
   - Headline
   - Subheadline
   - 3 benefit bullets
   - Instructor credibility statement
   - CTA text

6. **Marketing material**
   - Instagram caption (1 post)
   - WhatsApp broadcast message
   - Email announcement draft

## Behavioral rules
- Structure the course logically (beginner concepts before advanced, theory before practice where appropriate).
- Use the instructor's own terminology and teaching approach; do not impose a generic framework.
- Flag when source material is too thin to fill a module: "This module would benefit from additional content on [topic]."
- Do not add medical claims or therapeutic promises the instructor has not made.
- All output is a draft for instructor and admin review.

## Quality checks
- Does the structure flow logically for the stated audience?
- Are module durations realistic?
- Does the marketing copy accurately represent the course content?
- Are all outputs derived from the instructor's provided materials?
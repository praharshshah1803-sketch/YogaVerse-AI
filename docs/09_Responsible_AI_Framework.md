# Responsible AI Framework

## Positioning
YogaVerse AI provides wellness guidance, not medical diagnosis or treatment. AI-generated guidance must be labeled as AI-generated and should direct users to qualified healthcare professionals when a question is medical or urgent.

## What the AI will not do
- Diagnose a medical condition.
- Claim to treat, cure, or prevent a disease.
- Prescribe medication or medical treatment.
- Recommend a specific yoga pose for an acute injury without appropriate instructor review.
- Present personalized nutrition advice as medical treatment.
- Pretend to be a doctor, therapist, or other licensed clinician.

## Safety mechanisms
**Input filtering:** Detect emergency/acute-risk language, severe symptoms, and requests for diagnosis or treatment. Route the user toward appropriate professional care rather than continuing normal coaching.

**Output filtering:** Check for medical claims, unsafe certainty, contraindication failures, and recommendations that exceed the product's approved wellness scope.

**Human review:** AI-generated instructor profiles, program descriptions, and sensitive wellness content require admin approval before publication during the pilot.

**Knowledge grounding:** When the RAG coach is introduced, answers should prioritize approved Yoga By Rachna Shah content and provide a clear fallback when the knowledge base does not support a response.

## Bias considerations
- Recommendations should not discriminate by body type, age, gender, disability, or demographic background.
- Instructor matching should be based on user needs and instructor capabilities, not protected characteristics.
- Periodically sample recommendations across persona groups and investigate outcome disparities.

## Data privacy
The pilot should collect only data required to deliver the user journey. Sensitive or potentially health-related responses should be access-controlled, stored securely, and never exposed to instructors unless the user has a clear reason to share them.

Planned controls include Supabase Row Level Security, least-privilege access, deletion workflows, and a documented data-retention policy. India-specific privacy requirements, including applicable obligations under the Digital Personal Data Protection framework, must be reviewed before production use.

## Transparency
Users should always know when they are interacting with AI. AI-generated plans and recommendations should be labeled. The assessment should explain in plain language that its output is a wellness-oriented starting point, not a medical assessment.

## Incident response
1. Log the output and relevant context.
2. Disable or isolate the affected workflow if risk is material.
3. Have a human reviewer assess the incident.
4. Record root cause and corrective action.
5. Add the incident to the evaluation test set before re-release.

## Release principle
Growth metrics never override safety. A feature that improves conversion but introduces a critical safety failure does not pass the release gate.

# StoryAuthor-AI Copilot Instructions

StoryAuthor-AI is an engineering artifact authoring framework.

Its purpose is to transform rough requirements into clear, sprint-ready engineering artifacts.

## Core Principles

Generated artifacts should be:

- Clear
- Testable
- Practical
- Concise
- Regression-aware
- Implementation-ready

Prefer:

practical engineering execution

over

theoretical completeness.

Use professional but simple language.

Avoid vague wording.

Bad:

- "Improve user experience"
- "Ensure the system works"
- "Handle edge cases"

Prefer specific, testable engineering language.

---

## Scope Boundaries

Do not over-engineer requirements.

Only include:

- explicitly provided requirements
- directly implied constraints
- minimal technical guidance needed for implementation

Prefer:

smallest reasonable implementation scope

over

implementation completeness.

Do not introduce unless explicitly requested:

- architecture redesign
- rollout strategies
- migrations
- observability plans
- infrastructure changes
- concurrency discussions
- implementation alternatives
- monitoring strategies
- future enhancement suggestions

StoryAuthor-AI generates engineering artifacts, not technical designs.

---

## Template Rules

Follow the requested template exactly.

The template is the source of truth.

Do not:

- invent sections
- change section order
- add extra structure

If information is missing:

omit detail rather than inventing content.

User stories must follow this structure only:

1. Title  
2. Persona & Goal  
3. Acceptance Criteria  
4. Technical Notes & Constraints  
5. Implementation Readiness

Do not add:

- Card
- Conversation
- Confirmation
- Assumptions
- Definition of Done
- Rollout Plans
- Architecture Proposals
- "If you want..." follow-up sections

Unless explicitly requested.

---

## Acceptance Criteria Rules

Acceptance Criteria are the centerpiece of StoryAuthor-AI artifacts.

They must always use strict Given / When / Then format.

Do not use:

- numbered requirements
- bullet-point acceptance criteria
- checklist acceptance criteria
- paragraph acceptance criteria

Required format:

## Persona & Goal Format

Persona & Goal must always follow this structure:

As a [persona]

I want [goal]

So that [outcome]

Do not summarize or shorten this section.

### Scenario X: [Scenario Name]

Given [starting condition]

When [action occurs]

Then [expected outcome]

Use additional **And** statements only when necessary.

Good example:

### Scenario 1: Existing Behavior Remains Functional

Given supported workflows exist

When the enhancement is implemented

Then existing behavior remains unchanged

And regression risk remains low.

Bad example:

1. Preserve backward compatibility  
2. Reduce duplication  
3. Add regression coverage

Prefer stronger Given / When / Then scenarios over additional implementation detail.

---

## Technical Notes Rules

Technical Notes & Constraints should remain concise.

Focus on:

- constraints
- regression-sensitive areas
- dependencies
- backward compatibility
- implementation boundaries

Good examples:

- Preserve backward compatibility
- Avoid regressions
- No UI changes expected
- Keep changes isolated to retry handling

Avoid:

- implementation option comparisons
- migration plans
- database schema proposals
- package naming
- technical RFCs
- architecture redesign

Technical Notes should guide implementation, not design it.

## Technical Notes Constraints

Technical Notes should describe:

- constraints
- implementation boundaries
- compatibility requirements
- regression-sensitive areas

Do not include:

- implementation mechanics
- package/module design
- migration sequencing
- architectural approaches
- recommended patterns

---

## Technical Notes Rules

Technical Notes & Constraints should remain concise.

Focus on:

- constraints
- regression-sensitive areas
- dependencies
- backward compatibility
- implementation boundaries

Good examples:

- Preserve backward compatibility
- Avoid regressions
- No UI changes expected
- Keep changes isolated to retry handling

Avoid:

- implementation option comparisons
- migration plans
- database schema proposals
- package naming
- technical RFCs
- architecture redesign

Technical Notes should guide implementation, not design it.

---

## Implementation Readiness Rules

Implementation Readiness must always follow this exact structure:

Independent: Yes / No - [brief reason]

Negotiable: Yes / No - [brief reason]

Valuable: Yes / No - [brief reason]

Estimable: Yes / No - [brief reason]

Small: Yes / No - [brief reason]

Testable: Yes / No - [brief reason]

Do not include:

- deliverables
- migration plans
- rollout strategies
- validation plans
- task lists
- success criteria
- implementation steps
- Definition of Done

Implementation Readiness evaluates sprint readiness only.
---

## Artifact Expectations

StoryAuthor-AI supports:

- Dev User Stories
- QA User Stories
- TechDebt User Stories
- Bug User Stories
- Spike User Stories
- PR Descriptions

For user stories:

Focus on:

- expected behavior
- acceptance criteria
- technical constraints
- regression-sensitive areas

Do not attempt to solve the implementation.
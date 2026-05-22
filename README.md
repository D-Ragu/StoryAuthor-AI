# StoryAuthor-AI — Opinionated AI-Assisted User Story Generation

**Generate sprint-ready engineering user stories from rough requirements.**

StoryAuthor-AI is an opinionated framework for transforming incomplete engineering requirements into **clear, testable, sprint-ready user stories** using AI.

Built for engineers who are tired of:

- vague tickets
- weak acceptance criteria
- missing QA scope
- over-engineered AI output
- stories that are not sprint-ready

StoryAuthor-AI prioritizes:

- **behavior-first requirements**
- **strict Given / When / Then acceptance criteria**
- **regression awareness**
- **implementation boundaries**
- **low ambiguity**
- **engineering realism**

---

## 🤔 Why StoryAuthor-AI?

Most AI-generated user stories suffer from the same problems:

❌ Too vague  
❌ Too implementation-heavy  
❌ Missing QA considerations  
❌ Not sprint-ready  
❌ Poor acceptance criteria  
❌ Mini architecture documents disguised as tickets

StoryAuthor-AI solves this with an opinionated framework designed around **how engineers actually work**.

Instead of generating technical RFCs, StoryAuthor-AI produces:

> alignment artifacts engineers can realistically refine and drop into Jira or Azure DevOps.

---

## Supported Story Types

StoryAuthor-AI supports four engineering-focused user story types:

| Type | Purpose |
|-------|----------|
| Dev User Story | Sprint-ready implementation work |
| QA User Story | Validation and regression coverage |
| TechDebt User Story | Maintainability and engineering improvements |
| Bug User Story | Structured defect documentation |

All story types follow a consistent structure:

1. Title  
2. Persona & Goal  
3. Acceptance Criteria  
4. Technical Notes & Constraints  
5. Implementation Readiness

---

## Core Principles

StoryAuthor-AI is intentionally opinionated.

Generated stories should be:

### Clear

Requirements should be specific and understandable.

### Testable

Acceptance criteria must support validation.

### Practical

Stories should feel usable by engineering teams.

### Regression-Aware

Existing supported behavior matters.

### Low Ambiguity

Reduce guesswork during implementation.

### Behavior-First

Focus on expected outcomes before implementation details.

---

## Example

### Input

```text
We have duplicate retry logic spread across several services.

Retry behavior has drifted over time, making onboarding harder and increasing maintenance cost.

We want to improve consistency without changing observable behavior.

Requirements:
- preserve backward compatibility
- avoid major refactors
- low regression risk
```

### Prompt

```text
Use StoryAuthor-AI conventions.

Create a tech debt user story.
```

### Output (Excerpt)

```md
Title

Standardize retry behavior across services (Tech Debt)

Persona & Goal

As an engineer onboarding to the codebase

I want consistent, well-documented retry behavior across services

So that maintenance is easier, onboarding is faster, and behaviors remain predictable

Acceptance Criteria

Scenario 1: Preserve existing observable behavior

Given services currently have divergent retry behaviors in production

When a service adopts the standardized behavior

Then observable retry behavior remains unchanged
```

---

## Repository Structure

```text
storyauthor-ai/
│
├── .github/
│   └── copilot-instructions.md
│
├── prompts/
│   ├── dev-user-story.prompt.md
│   ├── qa-story.prompt.md
│   ├── tech-debt.prompt.md
│   └── bug-ticket.prompt.md
│
├── templates/
│   └── user-story-template.md
│
├── standards/
│   ├── engineering-principles.md
│   ├── given-when-then.md
│   ├── invest.md
│   └── three-cs.md
│
├── examples/
│   ├── dev-user-story-example.md
│   ├── qa-story-example.md
│   ├── tech-debt-example.md
│   └── bug-ticket-example.md
│
└── docs/
    ├── getting-started.md
    └── customization.md
```

---

## Quick Start

### 1. Clone the Repository

```bash
git clone https://github.com/D-Ragu/StoryAuthor-AI.git
```

### 2. Open the Repository in VS Code

GitHub Copilot works best when repository context is available.

StoryAuthor-AI includes:

```text
.github/copilot-instructions.md
```

to help steer output quality and formatting.

### 3. Choose a Story Type

Examples:

```text
prompts/dev-user-story.prompt.md
prompts/qa-story.prompt.md
prompts/tech-debt.prompt.md
prompts/bug-ticket.prompt.md
```

### 4. Paste a Rough Requirement

Example:

```text
We occasionally send duplicate password reset emails during retry failures.

Requirements:
- preserve current behavior
- low regression risk
- no UI changes
```

### 5. Generate a Story

Example prompt:

```text
Use StoryAuthor-AI conventions.

Create a bug user story.
```

---

## Engineering Standards

StoryAuthor-AI encourages:

### Given / When / Then

Acceptance criteria are written using strict behavioral scenarios:

```text
Scenario 1: Existing Behavior Remains Functional

Given supported workflows exist

When the enhancement is implemented

Then existing behavior remains unchanged
```

### Regression Awareness

Stories should preserve supported behavior whenever possible.

### Implementation Boundaries

Stories define:

> what engineering should align on

not

> how engineering must implement it

---

## Non-Goals

StoryAuthor-AI does **not** attempt to:

- replace engineers
- replace product managers
- generate production code
- generate architecture RFCs
- over-prescribe implementation

This project focuses on:

> improving engineering communication quality.

---

## Contributing

Contributions are welcome.

Areas of interest:

- better prompt patterns
- improved examples
- story quality improvements
- engineering workflow feedback

---

## License

MIT License

---

## Philosophy

StoryAuthor-AI favors:

> practical engineering execution

over

> theoretical completeness

A good user story should help engineering teams align quickly, reduce ambiguity, and move work forward.

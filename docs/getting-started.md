# Getting Started

StoryAuthor-AI is an opinionated framework for generating implementation-ready engineering artifacts using AI-assisted tooling such as GitHub Copilot, ChatGPT, Claude, or Cursor.

The goal is simple:

> Better engineering communication, faster.

StoryAuthor-AI helps standardize:

- Dev User Stories
- QA User Stories
- PR Descriptions
- TechDebt User Stories
- Bug User Stories

The framework emphasizes:

- Clear requirements
- Testable acceptance criteria
- Practical engineering communication
- Regression awareness
- Low ambiguity

---

# Prerequisites

StoryAuthor-AI works best with:

- GitHub Copilot
- ChatGPT
- Claude
- Cursor
- Any LLM capable of working with Markdown instructions

GitHub Copilot is the recommended starting point.

---

# Repository Structure

```txt
.github/
    copilot-instructions.md

prompts/
    dev-user-story.prompt.md
    qa-user-story.prompt.md
    tech-debt.prompt.md
    bug-ticket.prompt.md
    pr-description.prompt.md

templates/
    dev-user-story-template.md
    qa-story-template.md
    tech-debt-template.md
    bug-ticket-template.md
    pr-description-template.md

examples/
    example artifacts

standards/
    engineering-principles.md
    invest.md
    given-when-then.md
    three-cs.md
```

---

# How It Works

StoryAuthor-AI uses three layers:

### 1. Prompts

Prompts define:

- expected behavior
- writing style
- output expectations
- engineering principles

Example:

```txt
prompts/dev-user-story.prompt.md
```

---

### 2. Templates

Templates define:

- artifact structure
- required sections
- formatting consistency

Example:

```txt
templates/dev-user-story-template.md
```

---

### 3. Standards

Standards define:

- engineering philosophy
- writing expectations
- consistency rules

Example:

```txt
standards/engineering-principles.md
```

---

# Using StoryAuthor-AI with GitHub Copilot

StoryAuthor-AI works best inside a repository with:

```txt
.github/copilot-instructions.md
```

This helps GitHub Copilot understand:

- formatting expectations
- engineering principles
- output structure
- preferred writing style

Example prompt:

```txt
Create a sprint-ready dev user story.

Requirement:
Prevent duplicate notifications during retry scenarios.

Requirements:
- Preserve backward compatibility
- Avoid regressions
- Easy QA validation
```

Expected output:

- Persona & Goal
- Acceptance Criteria
- Technical Notes & Constraints
- Implementation Readiness

---

# Recommended Workflow

### Step 1: Start with a Dev User Story

Example:

```txt
Create a dev user story for implementing conditional MFA prompts.
```

---

### Step 2: Generate QA Coverage

Example:

```txt
Create a QA user story for the MFA implementation.
```

---

### Step 3: Implement the Work

Engineering completes development.

---

### Step 4: Generate a PR Description

Example:

```txt
Create a PR description for this change.
```

---

### Step 5: Refine if Needed

Adjust prompts or templates to better match your engineering organization.

StoryAuthor-AI is intentionally opinionated, but customizable.

---

# Example Artifacts

See:

```txt
examples/
```

For examples of:

- Dev User Stories
- QA User Stories
- PR Descriptions
- TechDebt Stories
- Bug Stories

---

# Philosophy

StoryAuthor-AI favors:

> practical engineering execution

over

> theoretical completeness

Generated artifacts should be:

- Clear
- Testable
- Practical
- Sprint-ready
- Low ambiguity

For more detail:

See:

```txt
standards/engineering-principles.md
```
# Customization

StoryAuthor-AI is intentionally opinionated.

However, every engineering organization writes artifacts differently.

This document explains how to customize StoryAuthor-AI for your team.

---

# Customization Philosophy

Customize:

- terminology
- structure
- wording
- engineering conventions

Do not customize:

- clarity
- testability
- practicality
- regression awareness

Those principles are core to StoryAuthor-AI.

---

# Customizing Templates

Templates define artifact structure.

Location:

```txt
templates/
```

Example:

```txt
templates/dev-user-story-template.md
```

You may customize:

- section names
- required sections
- formatting
- checklist requirements

Example:

Default:

```md
## Technical Notes & Constraints
```

Your organization:

```md
## Engineering Notes
```

---

# Customizing Prompts

Prompts control:

- tone
- output behavior
- complexity
- assumptions
- engineering depth

Location:

```txt
prompts/
```

Example:

Default:

```txt
Avoid speculative architecture discussions.
```

Your organization:

```txt
Include architecture considerations for platform work.
```

---

# Customizing Writing Style

Organizations often prefer different wording styles.

Example:

Default:

```txt
Then behavior continues functioning as expected.
```

Alternative:

```txt
Then the workflow shall remain unchanged.
```

StoryAuthor-AI intentionally defaults to modern engineering wording rather than enterprise-heavy process language.

---

# Customizing For Different Teams

### Product-Focused Teams

You may want:

- more business context
- customer impact
- success metrics

Add sections like:

```md
## Business Context
## Customer Impact
```

---

### Platform / Infrastructure Teams

You may want:

- architecture guidance
- operational concerns
- performance considerations

Add sections like:

```md
## Operational Impact
## Observability Considerations
```

---

### Enterprise Organizations

You may prefer:

- Definition of Done
- Readiness Gates
- Approval workflows

These can be added back into templates if needed.

---

# Adding New Artifact Types

StoryAuthor-AI currently supports:

- Dev User Story
- QA User Story
- PR Description
- TechDebt User Story
- Bug User Story

To add a new artifact:

### 1. Create a Prompt

Example:

```txt
prompts/spike-user-story.prompt.md
```

---

### 2. Create a Template

Example:

```txt
templates/spike-user-story-template.md
```

---

### 3. Add an Example

Example:

```txt
examples/spike-user-story-example.md
```

---

### 4. Update Documentation

Add the new artifact type to:

- README.md
- getting-started.md

---

# Recommendation

Start with the defaults.

Only customize after using StoryAuthor-AI for real engineering work.

Most teams over-customize too early.

The default structure is designed to balance:

- speed
- clarity
- consistency
- practicality
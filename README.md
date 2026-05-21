# StoryAuthor-AI

<p align="center">
  <h3 align="center">
    AI-Powered Engineering Artifact Authoring
  </h3>

  <p align="center">
    Transform rough requirements into sprint-ready engineering deliverables.
  </p>
</p>

---

## 🚀 What is StoryAuthor-AI?

**StoryAuthor-AI** is an open-source framework for generating **high-quality engineering artifacts using AI**.

Instead of spending time manually writing:

- User Stories
- QA Stories
- Tech Debt Tickets
- PR Descriptions
- Acceptance Criteria
- Sprint Review Scripts
- Release Notes

StoryAuthor-AI provides a **repeatable workflow system** that transforms rough requirements into **sprint-ready deliverables**.

Compatible with:

- GitHub Copilot
- ChatGPT
- Claude
- Cursor
- VS Code AI workflows
- Enterprise AI platforms

---

## 🤔 Why StoryAuthor-AI?

Engineering teams often lose time to inconsistent documentation.

Common problems:

❌ Poorly written Jira stories  
❌ Weak acceptance criteria  
❌ Missing QA scope  
❌ Inconsistent PR descriptions  
❌ Unclear technical requirements  
❌ Tickets that are not sprint-ready

Most AI-generated stories are too vague, too generic, or lack engineering rigor.

**StoryAuthor-AI fixes this with structured prompt workflows and reusable engineering standards.**

---

# ✨ Features

### Product & Agile Artifacts

✅ User Stories  
✅ QA Stories  
✅ Tech Debt Tickets  
✅ Bug Tickets  
✅ Acceptance Criteria  
✅ Suggested Subtasks  
✅ Sprint Review Scripts  
✅ Release Notes

### Engineering Workflows

✅ PR Description Authoring  
✅ Technical Context Injection  
✅ Risk Analysis Support  
✅ Testing Guidance  
✅ Sprint-Ready Formatting

### Built-in Standards

✅ INVEST-compliant stories  
✅ 3 C’s methodology  
✅ Given / When / Then acceptance criteria  
✅ Reusable engineering templates

---

# 🏗 Example Workflow

## Input

```text
Feature Request:
Prevent duplicate customer signatures
during XML generation edge cases.

Root Cause:
Duplicate writes may occur in rare
transaction execution paths.

Goal:
Prevent duplicate signatures without
changing existing system behavior.

Requirements:
- Maintain backward compatibility
- Avoid regressions
- Ensure easy QA validation
```

---

## Command

```text
/build-user-story
```

---

## Output

StoryAuthor-AI generates:

✅ Sprint-ready User Story  
✅ Acceptance Criteria  
✅ Suggested Subtasks  
✅ QA Story  
✅ PR Description  
✅ Sprint Review Script

---

# 🧱 Repository Structure

```text
storyauthor-ai/
│
├── prompts/
│   ├── user-story.prompt.md
│   ├── qa-story.prompt.md
│   ├── tech-debt.prompt.md
│   ├── bug-ticket.prompt.md
│   ├── pr-description.prompt.md
│   ├── sprint-review.prompt.md
│   └── release-notes.prompt.md
│
├── templates/
│   ├── user-story-template.md
│   ├── qa-story-template.md
│   ├── tech-debt-template.md
│   ├── bug-ticket-template.md
│   └── pr-description-template.md
│
├── standards/
│   ├── invest.md
│   ├── three-cs.md
│   ├── given-when-then.md
│   └── engineering-principles.md
│
├── examples/
│   ├── feature-story-example.md
│   ├── qa-story-example.md
│   ├── tech-debt-example.md
│   ├── pr-description-example.md
│   └── sprint-review-example.md
│
├── integrations/
│   ├── github-copilot/
│   ├── chatgpt/
│   ├── claude/
│   └── cursor/
│
└── docs/
    ├── getting-started.md
    ├── customization.md
    └── enterprise-adoption.md
```

---

# ⚡ Quick Start

## 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/StoryAuthor-AI.git
```

---

## 2. Choose an Artifact Type

Example:

```text
prompts/user-story.prompt.md
```

---

## 3. Paste Your Requirement

Example:

```text
We need to prevent duplicate signatures
from being written to XML during edge-case
transaction flows.

The solution must remain backward compatible
and easy to validate in QA.
```

---

## 4. Run With Your Preferred AI Assistant

Example prompt:

```text
Use user-story.prompt.md.

Generate a sprint-ready user story
from the following requirement:

[paste requirement here]
```

---

# 📋 Included Artifact Types

| Artifact | Purpose |
|----------|----------|
| User Story | Sprint-ready feature development |
| QA Story | Testing scope and validation |
| Tech Debt Story | Internal engineering improvements |
| Bug Ticket | Structured defect documentation |
| PR Description | Pull request communication |
| Sprint Review Script | Stakeholder demos |
| Release Notes | Change communication |

---

# 🧠 Engineering Standards

StoryAuthor-AI follows proven Agile and engineering practices.

## INVEST

Stories should be:

- **Independent**
- **Negotiable**
- **Valuable**
- **Estimable**
- **Small**
- **Testable**

---

## 3 C’s

Every story includes:

### Card
The requirement itself.

### Conversation
Supporting context and intent.

### Confirmation
Clear acceptance criteria.

---

## Given / When / Then

Acceptance criteria are structured for:

- Testability
- QA readiness
- Sprint execution
- Engineering clarity

---

# 🎯 Project Goals

StoryAuthor-AI aims to:

- Improve engineering communication
- Reduce ticket-writing overhead
- Improve sprint readiness
- Standardize engineering artifacts
- Increase delivery consistency
- Accelerate software delivery with AI

---

# 🚫 Non-Goals

StoryAuthor-AI does **not** aim to:

- Replace product managers
- Replace engineers
- Generate production code automatically
- Force a specific Agile methodology

Instead, it helps teams create **higher-quality engineering communication faster**.

---

# 🛣 Roadmap

## v1 — Foundation

- [ ] Prompt framework
- [ ] User story generation
- [ ] QA story generation
- [ ] Tech debt templates
- [ ] PR description workflows
- [ ] Standards library
- [ ] Example workflows

## v2 — Workflow Intelligence

- [ ] Multi-artifact generation
- [ ] Context-aware prompting
- [ ] Engineering persona support
- [ ] Output chaining

## v3 — Integrations

- [ ] GitHub Copilot workflows
- [ ] Jira integration
- [ ] Azure DevOps integration
- [ ] IDE workflows

---

# 🤝 Contributing

Contributions are welcome.

Ideas include:

- Better prompt patterns
- Additional artifact types
- Engineering templates
- AI integrations
- Workflow improvements

---

# 📜 License

MIT License

Use it. Improve it. Make engineering communication better.

---

## ⭐ If you find this useful

Consider starring the repository and contributing feedback.

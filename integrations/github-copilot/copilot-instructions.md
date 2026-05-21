@"
# GitHub Copilot Instructions

When working in this repository, treat StoryAuthor-AI as an engineering artifact authoring framework.

## General Rules

- Generate clear, sprint-ready engineering artifacts.
- Prefer practical delivery language over vague agile wording.
- Use Given / When / Then for acceptance criteria.
- Follow INVEST when generating user stories.
- Include QA considerations when relevant.
- Clearly call out assumptions.
- Do not invent business requirements.

## Preferred Outputs

- User stories
- QA stories
- Tech debt stories
- Bug tickets
- PR descriptions
- Sprint review scripts
- Release notes

## Tone

Professional, clear, direct, and implementation-ready.
"@ | Out-File -Encoding utf8 integrations\github-copilot\copilot-instructions.md
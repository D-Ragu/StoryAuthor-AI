name: QA Story
description: Create QA validation work
title: "[QA]: "
labels:
  - qa
body:
  - type: textarea
    id: feature
    attributes:
      label: Feature / Change
      description: What is being tested?
      placeholder: Link story or describe feature.
    validations:
      required: true

  - type: textarea
    id: scope
    attributes:
      label: Testing Scope
      description: What should QA validate?
      placeholder: Functional, regression, edge cases, negative testing.
    validations:
      required: true

  - type: textarea
    id: risks
    attributes:
      label: Regression Risks
      description: Areas most likely to break
      placeholder: Existing workflows impacted.

  - type: textarea
    id: notes
    attributes:
      label: Notes
      description: Additional QA guidance
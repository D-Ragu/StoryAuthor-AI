name: Bug Report
description: Report a defect
title: "[Bug]: "
labels:
  - bug
body:
  - type: textarea
    id: summary
    attributes:
      label: Summary
      description: What is broken?
    validations:
      required: true

  - type: textarea
    id: steps
    attributes:
      label: Steps to Reproduce
      placeholder: |
        1. Go to...
        2. Click...
        3. Observe...
    validations:
      required: true

  - type: textarea
    id: expected
    attributes:
      label: Expected Behavior
    validations:
      required: true

  - type: textarea
    id: actual
    attributes:
      label: Actual Behavior
    validations:
      required: true

  - type: textarea
    id: environment
    attributes:
      label: Environment
      placeholder: Browser, IDE, version, OS, etc.
name: Tech Debt
description: Engineering improvement or cleanup
title: "[TechDebt]: "
labels:
  - technical-debt
body:
  - type: textarea
    id: issue
    attributes:
      label: Current Problem
      description: What technical issue exists?
      placeholder: Describe the debt.
    validations:
      required: true

  - type: textarea
    id: impact
    attributes:
      label: Impact
      description: Why should we care?
      placeholder: Risk, velocity impact, maintainability, security.
    validations:
      required: true

  - type: textarea
    id: proposed_solution
    attributes:
      label: Proposed Solution
      description: Suggested fix or modernization
      placeholder: Refactor, upgrade, architecture changes.

  - type: textarea
    id: risks
    attributes:
      label: Risks / Considerations
      description: Known implementation concerns
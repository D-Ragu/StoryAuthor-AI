# [QA] Title

## Persona & Goal

As a QA engineer,

I want to validate [feature/change],

So that the implementation behaves correctly and regression risk is minimized.

---

## Overview

Briefly explain:

- What changed
- Why QA validation is needed
- Primary risks
- High-value validation areas

---

## Test Scope

### Functional Validation

Validate:

- Expected happy path behavior
- Business requirements
- User-facing functionality

### Regression Validation

Validate:

- Existing workflows remain unaffected
- Adjacent functionality still behaves correctly

### Edge Cases

Validate:

- Invalid inputs
- Boundary conditions
- Error handling
- Alternate workflows

### Negative Testing

Validate:

- Invalid usage
- Failure conditions
- Unexpected states

---

## Acceptance Criteria

### Scenario 1: Functional Validation

Given [starting condition]

When [feature/change is exercised]

Then [expected result occurs]

### Scenario 2: Regression Validation

Given existing supported functionality

When related workflows are exercised

Then behavior remains unchanged

### Scenario 3: Edge Case Validation

Given unexpected or invalid inputs

When the workflow executes

Then the system handles the scenario gracefully

---

## Test Data Requirements

- Sample data
- Edge case data
- Invalid data
- Regression datasets

---

## QA Notes

- High-risk areas
- Logging expectations
- Monitoring expectations
- Areas requiring extra attention

---

## Suggested QA Subtasks

- [ ] Review/update test cases
- [ ] Execute functional testing
- [ ] Execute regression testing
- [ ] Execute edge case validation
- [ ] Capture defects if needed
- [ ] Provide QA signoff notes

---

## Definition of Done

- [ ] Functional testing completed
- [ ] Regression testing completed
- [ ] Edge cases validated
- [ ] Defects documented
- [ ] QA signoff complete
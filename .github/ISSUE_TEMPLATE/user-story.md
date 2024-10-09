---
name: User Story
about: A template for capturing user stories with necessary details.
title: "[User Story] - <Brief Description>"
assignees: ""
labels: user story

---

body:
- type: markdown
  attributes:
    value: |
      ## User Story Template
      Fill in the details below to capture the user story correctly.

- type: input
  id: role
  attributes:
    label: User Role
    description: "Describe the user role (e.g., 'As a customer', 'As a developer')."
    placeholder: "As a [role]"
  validations:
    required: true

- type: input
  id: function
  attributes:
    label: Functionality Required
    description: "What functionality does this user require?"
    placeholder: "I need to [function]"
  validations:
    required: true

- type: input
  id: benefit
  attributes:
    label: Benefit
    description: "What benefit does the user achieve?"
    placeholder: "So that [benefit]"
  validations:
    required: true

- type: textarea
  id: details
  attributes:
    label: Details and Assumptions
    description: "Provide any additional details or assumptions."
    value: |
      * [document what you know]
  validations:
    required: false  # Optional field

- type: checkboxes
  id: acceptance-criteria
  attributes:
    label: Acceptance Criteria
    description: "List the acceptance criteria for this user story."
    options:
      - label: Given [some context]
        required: true
      - label: When [certain action is taken]
        required: true
      - label: Then [the outcome is observed]
        required: true
  validations:
    required: true

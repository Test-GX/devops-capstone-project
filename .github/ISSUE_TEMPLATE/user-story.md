---
name: User Story
about: A template for documenting user stories.
title: "[User Story] - <Brief Description>"
assignees: ""
labels: user story

---

body:
# User Story Details
- type: markdown
  attributes:
    value: |
      Please fill out the following fields to provide full context for the user story.

- type: input
  id: role
  attributes:
    label: Role
    description: "Specify the user role that will benefit from this story (e.g., 'Customer', 'Admin')."
    placeholder: "Customer"
  validations:
    required: true

- type: input
  id: function
  attributes:
    label: Function
    description: "Specify the function that is required."
    placeholder: "I need to be able to create an account."
  validations:
    required: true
    
- type: input
  id: benefit
  attributes:
    label: Benefit
    description: "What benefit does this function provide?"
    placeholder: "So that I can access my account."
  validations:
    required: true

- type: textarea
  id: details
  attributes:
    label: Details and Assumptions
    description: "Provide any additional details or assumptions about the user story."
    value: |
      * [Write here any known details and assumptions.]
  validations:
    required: false

- type: markdown
  attributes:
    value: |
      ### Acceptance Criteria
      Use the format below to outline the acceptance criteria for this user story.
  
- type: textarea
  id: acceptance-criteria
  attributes:
    label: Acceptance Criteria
    description: "Provide acceptance criteria using Gherkin format."
    value: |
      Given [some context]
      When [certain action is taken]
      Then [the outcome is observed]
    render: bash
  validations:
    required: true

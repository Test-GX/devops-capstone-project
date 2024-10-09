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
        **As a** [role]  
        **I need** [function]  
        **So that** [benefit]  

  - type: textarea
    id: assumptions
    attributes:
      label: Details and Assumptions
      description: "Document any assumptions or additional details here."
      value: |
        * [document what you know]
    validations:
      required: false

  - type: textarea
    id: acceptance-criteria
    attributes:
      label: Acceptance Criteria  
      description: "Define the acceptance criteria using Gherkin syntax."
      value: |
        Given [some context]  
        When [certain action is taken]  
        Then [the outcome of action is observed]
    validations:
      required: true

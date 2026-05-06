name: 📋 Task
description: A discrete piece of work (smaller than an epic)
labels: []
body:
  - type: markdown
    attributes:
      value: |
        ### Use this for discrete, actionable work items.
  - type: dropdown
    id: issue_type
    attributes:
      label: Issue Type
      description: What type of issue is this?
      options:
        - Task
      default: 0
    validations:
      required: true
  - type: dropdown
    id: priority
    attributes:
      label: Priority
      options:
        - P0
        - P1
        - P2
        - P3
      default: 2
    validations:
      required: true
  - type: dropdown
    id: size
    attributes:
      label: Size
      options:
        - XS
        - S
        - M
        - L
        - XL
      default: 2
    validations:
      required: true
  - type: input
    id: component
    attributes:
      label: Component / Repo
      placeholder: e.g., engine-core
  - type: textarea
    id: description
    attributes:
      label: Description
      description: What needs to be done?
      placeholder: Clear, actionable description...
    validations:
      required: true
  - type: textarea
    id: acceptance
    attributes:
      label: Acceptance Criteria
      value: |
        - [ ] 
    validations:
      required: false
  - type: textarea
    id: notes
    attributes:
      label: Notes
      description: Any relevant context or references

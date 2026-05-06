name: 📐 Epic
description: Define a large body of work spanning multiple issues or repos
labels: ["epic"]
body:
  - type: markdown
    attributes:
      value: |
        ### Epics are large initiatives that span multiple issues and potentially multiple repos.
        Use this template to define scope, goals, and acceptance criteria.
  - type: dropdown
    id: issue_type
    attributes:
      label: Issue Type
      description: What type of issue is this?
      options:
        - Epic
      default: 0
    validations:
      required: true
  - type: dropdown
    id: priority
    attributes:
      label: Priority
      description: How important is this epic?
      options:
        - P0 - Critical (blocks roadmap)
        - P1 - High (key initiative)
        - P2 - Normal
        - P3 - Low
      default: 2
    validations:
      required: true
  - type: input
    id: component
    attributes:
      label: Component / Repo
      description: Which repos or components are involved?
      placeholder: e.g., engine-core + auth-service + docs
  - type: textarea
    id: goal
    attributes:
      label: Goal
      description: What are we trying to achieve?
      placeholder: Define the outcome, not the solution...
    validations:
      required: true
  - type: textarea
    id: scope
    attributes:
      label: Scope
      description: What's in and out of scope?
      value: |
        #### In Scope
        - 

        #### Out of Scope
        - 
    validations:
      required: true
  - type: textarea
    id: acceptance
    attributes:
      label: Acceptance Criteria
      description: What needs to be true for this epic to be considered done?
      value: |
        - [ ] 
        - [ ] 
        - [ ] 
  - type: textarea
    id: related
    attributes:
      label: Related Issues / PRs
      description: Link to any related issues, PRs, or docs
  - type: textarea
    id: notes
    attributes:
      label: Notes
      description: Any additional context, decisions, or references

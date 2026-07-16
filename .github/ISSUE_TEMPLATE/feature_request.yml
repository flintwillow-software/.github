name: ✨ Feature Request
description: Propose a new feature or enhancement
labels: ["enhancement"]
body:
  - type: markdown
    attributes:
      value: |
        ### Before you begin
        Please search to see if an issue already exists for this feature.
  - type: dropdown
    id: issue_type
    attributes:
      label: Issue Type
      description: What type of issue is this?
      options:
        - Feature
      default: 0
    validations:
      required: true
  - type: dropdown
    id: priority
    attributes:
      label: Priority
      description: How important is this feature?
      options:
        - P0 - Critical (blocks core workflow)
        - P1 - High (major user need)
        - P2 - Normal (nice to have)
        - P3 - Low (minor improvement)
      default: 2
    validations:
      required: true
  - type: dropdown
    id: size
    attributes:
      label: Size
      description: Estimated effort to implement
      options:
        - XS - Under 1 hour
        - S - 1-2 hours
        - M - Half day
        - L - 1-2 days
        - XL - 3+ days
      default: 2
    validations:
      required: true
  - type: input
    id: component
    attributes:
      label: Component / Repo
      description: Which repo or component would this affect?
      placeholder: e.g., engine-core, docs, tooling
  - type: textarea
    id: problem
    attributes:
      label: Problem
      description: What problem does this feature solve?
      placeholder: I'm always frustrated when...
    validations:
      required: true
  - type: textarea
    id: solution
    attributes:
      label: Proposed Solution
      description: How do you envision this working?
      placeholder: Describe the feature behavior...
    validations:
      required: true
  - type: textarea
    id: alternatives
    attributes:
      label: Alternatives Considered
      description: What alternatives have you considered?
  - type: textarea
    id: context
    attributes:
      label: Additional Context
      description: Add any other context, links to related issues, or screenshots
  - type: checkboxes
    id: acknowledgements
    attributes:
      label: Acknowledgements
      description: Please read this carefully.
      options:
        - label: I have searched the existing issues
          required: true
        - label: I have confirmed this feature doesn't already exist
          required: true

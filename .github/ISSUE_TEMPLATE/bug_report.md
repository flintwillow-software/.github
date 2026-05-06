name: 🐛 Bug Report
description: File a bug report
labels: ["bug"]
body:
  - type: markdown
    attributes:
      value: |
        ### Before you begin
        Please search to see if an issue already exists for this bug.
  - type: dropdown
    id: issue_type
    attributes:
      label: Issue Type
      description: What type of issue is this?
      options:
        - Bug
      default: 0
    validations:
      required: true
  - type: dropdown
    id: priority
    attributes:
      label: Priority
      description: How urgent or impactful is this bug?
      options:
        - P0 - Critical (system down, data loss, security)
        - P1 - High (major feature broken, no workaround)
        - P2 - Normal (standard bug)
        - P3 - Low (minor, cosmetic, edge case)
      default: 2
    validations:
      required: true
  - type: dropdown
    id: size
    attributes:
      label: Size
      description: Estimated effort to resolve
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
      description: Which repo or component does this affect?
      placeholder: e.g., engine-core, auth-service
  - type: textarea
    id: what-happened
    attributes:
      label: What happened?
      description: Also tell us, what did you expect to happen?
      placeholder: Tell us what you see!
      value: |
        #### Steps to Reproduce

        1. 
        2. 
        3. 

        #### Expected Behavior

        #### Actual Behavior
    validations:
      required: true
  - type: textarea
    id: screenshots
    attributes:
      label: Screenshots / Screenshots
      description: If applicable, drag and drop screenshots or links to them
      placeholder: Paste images here
    validations:
      required: false
  - type: textarea
    id: logs
    attributes:
      label: Relevant log output
      description: Please copy and paste any relevant log output. This will be automatically formatted into code.
      render: shell
  - type: checkboxes
    id: acknowledgements
    attributes:
      label: Acknowledgements
      description: Please read this carefully to ensure the issue is complete.
      options:
        - label: I have searched the existing issues
          required: true
        - label: I have confirmed this bug exists in the latest version
          required: false

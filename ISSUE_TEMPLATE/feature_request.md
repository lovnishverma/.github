name: 🚀 Feature Request
description: Suggest an idea for this project
title: "[FEATURE] "
labels: ["enhancement", "needs-triage"]
assignees:
  - lovnishverma
body:
  - type: markdown
    attributes:
      value: |
        Thanks for suggesting a new feature! 🚀
        
  - type: checkboxes
    id: checklist
    attributes:
      label: Pre-submission Checklist
      description: Please ensure you've completed these steps
      options:
        - label: I have searched existing issues to avoid duplicates
          required: true
        - label: I have checked if this feature already exists
          required: true
        - label: This is not a bug report (use Bug Report template)
          required: true

  - type: textarea
    id: problem
    attributes:
      label: 🤔 Problem Statement
      description: Is your feature request related to a problem? Please describe.
      placeholder: "I'm always frustrated when..."
    validations:
      required: true

  - type: textarea
    id: solution
    attributes:
      label: 💡 Proposed Solution
      description: Describe the solution you'd like
      placeholder: "I would like to see..."
    validations:
      required: true

  - type: textarea
    id: alternatives
    attributes:
      label: 🔄 Alternatives Considered
      description: Describe alternatives you've considered
      placeholder: "I also considered..."

  - type: dropdown
    id: priority
    attributes:
      label: 📈 Priority
      description: How important is this feature to you?
      options:
        - Low - Nice to have
        - Medium - Would improve my workflow
        - High - Would significantly impact my work
        - Critical - Blocking my progress
    validations:
      required: true

  - type: textarea
    id: implementation
    attributes:
      label: 🛠️ Implementation Ideas
      description: Do you have ideas on how this could be implemented?
      placeholder: "This could be implemented by..."

  - type: textarea
    id: additional
    attributes:
      label: 📄 Additional Context
      description: Add any other context or screenshots about the feature request
      placeholder: "Any additional information, mockups, or examples..."

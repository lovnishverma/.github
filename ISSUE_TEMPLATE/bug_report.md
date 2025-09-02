```yaml
name: "🐛 Bug Report"
description: "Create a report to help us improve"
title: "[BUG] "
labels: ["bug", "needs-triage"]
assignees:
  - lovnishverma

body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this bug report! 🐛
        
  - type: checkboxes
    id: checklist
    attributes:
      label: "Pre-submission Checklist"
      description: "Please ensure you've completed these steps"
      options:
        - label: "I have searched existing issues to avoid duplicates"
          required: true
        - label: "I have read the contributing guidelines"
          required: true
        - label: "This is not a question (use Discussions for questions)"
          required: true

  - type: textarea
    id: description
    attributes:
      label: "📝 Bug Description"
      description: "A clear and concise description of what the bug is"
      placeholder: "Describe the bug..."
    validations:
      required: true

  - type: textarea
    id: reproduction
    attributes:
      label: "🔄 Steps to Reproduce"
      description: "Steps to reproduce the behavior"
      placeholder: |
        1. Go to '...'
        2. Click on '...'
        3. Scroll down to '...'
        4. See error
    validations:
      required: true

  - type: textarea
    id: expected
    attributes:
      label: "✅ Expected Behavior"
      description: "What you expected to happen"
      placeholder: "Describe what should have happened..."
    validations:
      required: true

  - type: textarea
    id: actual
    attributes:
      label: "❌ Actual Behavior"
      description: "What actually happened"
      placeholder: "Describe what actually happened..."
    validations:
      required: true

  - type: textarea
    id: screenshots
    attributes:
      label: "📸 Screenshots/Videos"
      description: "If applicable, add screenshots or videos to help explain your problem"
      placeholder: "Drag and drop images or paste URLs here..."

  - type: dropdown
    id: os
    attributes:
      label: "🖥️ Operating System"
      description: "What operating system are you using?"
      options:
        - Windows
        - macOS
        - Linux (Ubuntu)
        - Linux (Other)
        - iOS
        - Android
        - Other
    validations:
      required: true

  - type: input
    id: version
    attributes:
      label: "📦 Version"
      description: "What version of the software are you running?"
      placeholder: "e.g., v1.2.3"
    validations:
      required: true

  - type: dropdown
    id: browser
    attributes:
      label: "🌐 Browser (if applicable)"
      description: "If this is a web-related bug, which browser?"
      options:
        - Chrome
        - Firefox
        - Safari
        - Edge
        - Opera
        - Other
        - Not applicable

  - type: textarea
    id: logs
    attributes:
      label: "📋 Error Logs"
      description: "Please copy and paste any relevant log output"
      render: shell
      placeholder: "Paste error logs here..."

  - type: textarea
    id: additional
    attributes:
      label: "📄 Additional Context"
      description: "Add any other context about the problem here"
      placeholder: "Any additional information that might be helpful..."
```
Do you also want me to create **separate templates for Feature Requests and Questions** (so your repo has a complete issue flow), or just keep it limited to bug reports?

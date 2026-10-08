---
name: Icon Request
about: Request a new icon
title: "[Icon Request] "
labels: ["icon-request"]
assignees: []
body:
  - type: input
    id: name
    attributes:
      label: Suggested name
      description: English kebab-case, e.g. user-pen, cloud-database. Match the existing naming style.
      placeholder: e.g. cloud-function
    validations:
      required: true

  - type: input
    id: category
    attributes:
      label: Suggested category
      description: Which of the 34 categories it belongs to. Browse them at https://qingicon.com.
      placeholder: e.g. Cloud / AI / General
    validations:
      required: true

  - type: textarea
    id: usage
    attributes:
      label: Use case
      description: Where will this icon be used? What problem does it solve? The more specific, the more likely it gets accepted.
      placeholder: Describe your use case...
    validations:
      required: true

  - type: dropdown
    id: variant
    attributes:
      label: Expected style
      options:
        - Line
        - Fill
        - Both
    validations:
      required: true

  - type: textarea
    id: reference
    attributes:
      label: References
      description: Paste reference screenshots, links to similar icons, or a sketch. Optional but strongly recommended.
      placeholder: Drag images here, or paste links...
    validations:
      required: false

  - type: checkboxes
    id: urgent
    attributes:
      label: Priority
      options:
        - label: This is urgent and I hope it gets supported soon
          required: false
---


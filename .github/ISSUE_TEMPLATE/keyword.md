---
name: Keyword Suggestion
about: Add Chinese / English search keywords to an existing icon
title: "[Keyword] "
labels: ["keyword"]
assignees: []
body:
  - type: input
    id: icon
    attributes:
      label: Icon name
      description: The existing icon to add keywords to (e.g. user-pen). Copy it from the icon detail page on the website.
      placeholder: e.g. user-pen
    validations:
      required: true

  - type: textarea
    id: zh
    attributes:
      label: Chinese keywords to add
      description: One per line, or comma-separated. Use words people would actually search.
      placeholder: |
        用户
        个人
        账号
      render: markdown
    validations:
      required: false

  - type: textarea
    id: en
    attributes:
      label: English keywords to add
      description: One per line, or comma-separated. Use kebab-case (e.g. user-account).
      placeholder: |
        user
        account
        profile
      render: markdown
    validations:
      required: false

  - type: textarea
    id: note
    attributes:
      label: Notes
      description: Why add these words? Any synonyms/ambiguities to note? Optional.
      placeholder: These words are easily confused with xxx in search...
    validations:
      required: false
---


name: Pull Request
description: Fill out the PR template to describe changes.
title: "[PR]: " # Pre-fill PR title
body:
- type: input
  id: pr_title
  attributes:
  label: "🔖 PR Title"
  description: "Provide a short and clear PR title."
  placeholder: "Enter PR title here"

- type: textarea
  id: summary
  attributes:
  label: "📌 Summary"
  description: "Provide a concise summary of the changes made in this PR."
  placeholder: "Enter summary here"

- type: checkboxes
  id: changes
  attributes:
  label: "🔄 Changes Introduced"
  description: "Select the changes introduced in this PR."
  options:
  - label: "Feature"
  - label: "Bug fix"
  - label: "Refactoring"
  - label: "Documentation updates"

- type: textarea
  id: testing
  attributes:
  label: "🛠️ How Has This Been Tested?"
  description: "Describe the testing strategy used for this PR."
  placeholder: "Enter testing details here"

- type: input
  id: jira_ticket
  attributes:
  label: "🎯 Related JIRA/Ticket"
  description: "Add links to related tickets or issues."
  placeholder: "Enter JIRA ticket or issue number"

- type: checkboxes
  id: code_review
  attributes:
  label: "🔍 Code Review Checklist"
  description: "Ensure best practices are followed."
  options:
  - label: "Code follows best practices"
  - label: "No hardcoded values"
  - label: "Proper logging and error handling"
  - label: "Security considerations addressed"
  - label: "Performance impact considered"

- type: textarea
  id: additional_notes
  attributes:
  label: "📝 Additional Notes"
  description: "Add any other relevant information."
  placeholder: "Enter additional notes here"

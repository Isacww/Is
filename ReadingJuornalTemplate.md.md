---
date: <% tp.date.now("YYYY-MM-DD") %>  <!-- Auto-inserts current date for dynamism -->
book: <% tp.user.prompt("Enter the book title:") %>  <!-- Prompts for book title -->
tags: <% tp.user.prompt("Enter tags (comma-separated):") %>  <!-- Another prompt for tags -->
---
# Reading Journal: <%- tp.user.prompt("Enter the book title:") %>  <!-- Reuses the prompt if needed, but better to store in a variable -->

## Key Phrase/Quote
[Paste quote here]

## My Connection
[Your insight, e.g., links to Tesla's 369 or da Vinci's geometry]

## Synchronicities
- [List unexpected ways this found you]

## Cross-References
- [[RelatedNote1.md|Link to Emerald Tablet parallels]]
- [[RelatedNote2.md|Link to Ringing Cedars dolmens]]

## Next Actions
- [Books/ideas this sparks]
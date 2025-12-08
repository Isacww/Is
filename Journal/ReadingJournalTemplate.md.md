
date: <% tp.date.now("YYYY-MM-DD") %>
book: <% tp.user.prompt("Enter the book title:") %>
tags: <% tp.user.prompt("Enter tags (comma-separated):") %>

# Reading Journal: <%- tp.user.prompt("Enter the book title:") %>

## Key Phrase/Quote
[]

## My Connection
[Your insight, e.g., links to Tesla's 369 or da Vinci's geometry]

## Synchronicities
- [List unexpected ways this found you]

## Cross-References
- [[RelatedNote1.md|Link to Emerald Tablet parallels]]
- [[RelatedNote2.md|Link to Ringing Cedars dolmens]]

## Next Actions
- [Books/ideas this sparks]

File creation date:  <% tp.file.creation_date() %>
Last Modified:  <% tp.file.last_modified_date() %>
File folder:  <% tp.file.folder %>
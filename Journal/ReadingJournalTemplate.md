<%*
const book = await tp.user.prompt("Enter the book title:");
const tags_input = await tp.user.prompt("Enter tags (comma-separated):");

// turn "tag1, tag2" into ["tag1", "tag2"]
const tags = tags_input
  ? tags_input.split(",").map(t => t.trim()).filter(t => t.length > 0)
  : [];

tR += `---
date: ${tp.date.now("YYYY-MM-DD")}
book: "${book || ""}"
tags: [${tags.map(t => `"${t}"`).join(", ")}]
---

`;
%>

# Reading Journal:

## Key Phrase/Quote
- [Paste quote here]
## My Connection
- [Your insight, e.g., links to Tesla's 369 or da Vinci's geometry]
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
<%*
const book = await tp.user.prompt("Book title?");
const date = tp.date.now("YYYY-MM-DD");

await tp.file.rename(`${book} - ${date}`);
%>
---
date: <% tp.date.now("YYYY-MM-DD") %>
book: "<%* book %>"
tags:
---
## Key Phrase/Quote
<!-- Paste quote here -->

## My Connection
<!-- Your insights (Tesla 369, da Vinci geometry, etc.) -->

## Synchronicities
<!-- List unexpected events or connections -->

## Cross-References
<!-- Add useful related notes here -->

## Next Actions
<!-- Books, ideas, or things to pursue -->

File creation date: 2025-12-08 14:58
Last Modified: 2025-12-08 15:37

<%*
let book = await tp.system.prompt("Article title?");
if (!book) book = "Untitled";

const date = tp.date.now("YYYY-MM-DD");

// rename file automatically
await tp.file.rename(`${book} - ${date}`);
%>---
date: <% date %>
book: "<% book %>"
tags: article
---

## Key Phrase/Quote
<!-- paste quote -->

## My Connection
<!-- your insights -->

## Synchronicities
<!-- events that lined up -->

## Cross-References
<!-- add related notes -->

## Next Actions
<!-- ideas sparked -->

File creation date: <% tp.file.creation_date() %>  
Last Modified: <% tp.file.last_modified_date() %>
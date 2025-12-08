<%*
let area = await tp.system.prompt("What is the question about?");
if (!area) area = "Untitled";

const date = tp.date.now("YYYY-MM-DD");

// rename file automatically
await tp.file.rename(`${area} - ${date}`);
%>---
date: <% date %>
Area: "<% area %>"
tags: question
---
## My Question
<!-- your insights -->

## Reason why it appeared:
<!-- events that lined up -->

## Cross-References
<!-- add related notes -->

## Next Actions
<!-- ideas sparked -->

File creation date: <% tp.file.creation_date() %>  
Last Modified: <% tp.file.last_modified_date() %>
<%*
let area = await tp.system.prompt("What is the thought about?");
if (!area) area = "Untitled";

const date = tp.date.now("YYYY-MM-DD");

// rename file automatically
await tp.file.rename(`${area} - ${date}`);
%>---
date: <% date %>
Thought: "<% area %>"
tags:
---
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
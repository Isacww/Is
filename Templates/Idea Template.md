<%*
let area = await tp.system.prompt("What is the idea about?");
if (!area) area = "Untitled";

const date = tp.date.now("YYYY-MM-DD");

// rename file automatically
await tp.file.rename(`${area} - ${date}`);
%>---
date: <% date %>
Idea: "<% area %>"
tags: idea
---
## My Connection
<!-- your insights -->
## Description of the idea:
<!-- idea here -->
## Next Actions
<!-- ideas sparked -->

File creation date: <% tp.file.creation_date() %>  
Last Modified: <% tp.file.last_modified_date() %>
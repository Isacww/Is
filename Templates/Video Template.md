<%*
let video = await tp.system.prompt("Video title?");
if (!video) video = "Untitled";

const date = tp.date.now("YYYY-MM-DD");

// rename file automatically
await tp.file.rename(`${video} - ${date}`);
%>---
date: <% date %>
video: "<% video %>"
tags: video
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
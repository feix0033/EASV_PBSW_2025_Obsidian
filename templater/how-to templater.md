---
title: <% tp.file.title %>
create_date: <% tp.file.creation_date("DD-MM-YYYY HH:mm") %>
last_modify_date: <% tp.file.last_modified_date("DD-MM-YYYY HH:mm") %>
descriptions: 
summary: []
references:
---

<% tp.file.cursor() %>
<% await tp.file.move("/how-to/" + tp.file.path(true)) %>
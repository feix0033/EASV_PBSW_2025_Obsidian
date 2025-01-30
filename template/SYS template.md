---
title: <% tp.file.title %>
create_date: <% tp.file.creation_date("DD-MM-YYYY HH:mm") %>
last_modify_date: <% tp.file.last_modified_date("DD-MM-YYYY HH:mm") %>
aliases: 
tags: 
references:
---
<% tp.file.cursor() %>
<% await tp.file.move("notes/SYS" + tp.file.title) %>
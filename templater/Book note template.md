---
title: <% tp.file.title %>
tags: 
aliases: 
create_date: <% tp.file.creation_date("DD-MM-YYYY HH:mm") %>
last_modify_date: <% tp.file.last_modified_date("DD-MM-YYYY HH:mm") %>
references: 
describetion:
annotation-target: 
---
<% tp.file.cursor() %>
<% await tp.file.move("/books/" + tp.file.path(true)) %>


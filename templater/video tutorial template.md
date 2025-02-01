---
title: <% tp.file.title %>
create_date: <% tp.file.creation_date("DD-MM-YYYY HH:mm") %>
last_modify_date: <% tp.file.last_modified_date("DD-MM-YYYY HH:mm") %>
video: 
aliases: 
tags:
  - toturial
  - video
---
<% tp.file.cursor() %>
<% await tp.file.move("tutorial/" + tp.file.title + "/" + tp.file.title) %>

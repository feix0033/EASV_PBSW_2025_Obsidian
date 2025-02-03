---
date: <% tp.file.creation_date("DD-MM-YYYY HH:mm") %>
---
# <% tp.date.now("dddd, LL")%>, Week: <% tp.date.now("Wo")%> 

<< [[<% tp.date.now("DD-MM-YYYY", -1, tp.file.title, "DD-MM-YYYY") %>]] | [[<% tp.date.now("DD-MM-YYYY", +1, tp.file.title, "DD-MM-YYYY") %>]] >>
***
```tasks
not done
```
---
<% tp.file.cursor() %>


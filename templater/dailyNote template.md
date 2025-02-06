---
date: <% tp.file.creation_date("DD-MM-YYYY HH:mm") %>
---
---
date: <% tp.file.creation_date("DD-MM-YYYY HH:mm") %>
---
# <% tp.date.now("dddd, LL")%>, Week: <% tp.date.now("Wo")%> 

>[!quate] << [[<% tp.date.now("DD-MM-YYYY", -1, tp.file.title, "DD-MM-YYYY") %>]] | [[<% tp.date.now("DD-MM-YYYY", +1, tp.file.title, "DD-MM-YYYY") %>]] >>
***
> [!abstract]
```dataviewjs
const term ="#abstract"
let folderpath="journals"
const files = app.vault.getMarkdownFiles().filter(file=>file.path.includes(folderpath))
const arr = files.map(async ( file) => {
const content = await app.vault.cachedRead(file)
const lines = content.split("\n").filter(line => line.contains(term))
return lines
})
Promise.all(arr).then(values => 
dv.list(values.flat())) 
```
***
> [!TODO]
> ```tasks
> not done
> description does not include #archive
> ```
***
<% tp.file.cursor() %>

---
title: <% tp.file.title %>
created: <% tp.file.creation_date() %>
tags:
  - Journal
  - Tasks
status: ongoing
cssclasses:
  - img-rounded
  - img-centered
---

Task Located In:
```dataview
LIST
from #daily
where contains(file.outlinks, this.file.link) 
sort file.name ASC
```
---


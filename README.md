# Reading Books

```dataview
table publisher, author, status
from #book
where file.folder = "02-Book" and status != "done"
```


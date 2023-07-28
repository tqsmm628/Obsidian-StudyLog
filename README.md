# Reading Books

```dataview
table source, publisher, status
from #book
where file.folder = "02-Book" and status != "done"
```


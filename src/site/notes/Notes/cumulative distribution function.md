```dataview
list
from 
where file.ctime >= date(today) - dur(10 day)
sort file.ctime asc

```
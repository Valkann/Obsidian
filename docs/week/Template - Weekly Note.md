```dataview
table type, rating, summary, file.cday as date
from (#finished or #reading ) and (#article or #book or #SN/Article or #SN/Livre or #SN/Newsletter)
where contains(Week,<% tp.date.now("WW") %>)
sort file.cday
```
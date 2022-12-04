```dataview
table type, rating, summary, file.cday as date
from (#finished or #reading ) and (#article or #book or #SN/Article or #SN/Livre )
where contains(Week,{{date:WW}})
sort file.cday
```
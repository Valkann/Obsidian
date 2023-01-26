---
share: true 
category: source/livres
date: {{DATE:YYYY-MM-DD}}
updated: {{DATE:YYYY-MM-DD HH:mm:ss}}
banner: {{coverUrl}}
---
title:: "<% tp.file.title %>"
Date:: <% tp.date.now("YYYY-MM-DD") %>
Week:: [<% tp.date.now("YYYY-WW") %>](%3C%25%20tp.date.now(%22YYYY-WW%22)%20%25%3E.md)
Author:: [{{author}}](%7B%7Bauthor%7D%7D.md)
publisher:: {{publisher}}
publish:: {{publishDate}}
total:: {{totalPage}}
isbn:: {{isbn10}} {{isbn13}}


Type:: #SN/Livre 
Status:: #WiP 

![cover|150]({{coverUrl}})

# {{title}}

{{description}}
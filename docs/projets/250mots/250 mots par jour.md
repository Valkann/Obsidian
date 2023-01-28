```dataview
TABLE jour as Jour, mots as Mots
FROM #250mots 
WHERE !contains(file.name, "Template")
SORT jour
```
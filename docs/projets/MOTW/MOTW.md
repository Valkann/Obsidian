```dataviewjs
for (let group of dv.pages("#MotW").groupBy(p => p.type)) {

    dv.header(3, group.key);

    dv.table(["Note(s) - ", "Type", "status"],

        group.rows

            .sort(k => k.type, 'type')

            .map(k => [k.file.link, k["type"], k["status"]]));

}
```
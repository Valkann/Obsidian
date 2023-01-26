```dataviewjs
for (let group of dv.pages("#MotW").groupBy(p => p.type)) {

    dv.header(3, group.key);

    dv.table(["Name", "Type"],

        group.rows

            .sort(k => k.type, 'type')

            .map(k => [k.file.link, k["type"]]));

}
```
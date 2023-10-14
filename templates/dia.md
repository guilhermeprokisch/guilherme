<%*
await tp.file.move(`/guilherme/dias/${tp.file.title}`);
-%>
<%*
let today = moment(tp.file.title);
tR += '[[' + today.subtract(1, 'days').format('YYYY-MM-DD') + ']]';
tR += ' | [[' + today.add(2, 'days').format('YYYY-MM-DD') + ']]';
today.subtract(0, 'days');
%>

<% tp.file.cursor() %>


---
### Notes created today
```dataview
List FROM "" WHERE file.cday = date("<% tp.file.creation_date("YYYY-MM-DD") %>") SORT file.ctime asc
```

### Notes last touched today
```dataview
List FROM "" WHERE file.mday = date("<%tp.date.now("YYYY-MM-DD")%>") SORT file.mtime asc
```
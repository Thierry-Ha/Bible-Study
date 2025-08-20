# TO-Listen ect
```dataview 
table file.mtime.year as MY, file.mtime.month as MM, file.mtime.day as MD
from #To 
WHERE file.name != "Template Podcast"
sort file.ctime asc
``` 



# Zettelkasten
## - 🌱️
```dataview 
table file.mtime.year as MY, file.mtime.month as MM, file.mtime.day as MD, Status
from #🧠/📥/📝/🌱   AND !#🧠/🗺️ 
sort file.ctime asc
``` 


### Notes: 
```dataview 
table file.mtime.year as MY, file.mtime.month as MM, file.mtime.day as MD
from #🧠/📥/📝  AND #🟥
sort file.ctime asc
``` 
### Podcasts

```dataview 
table file.mtime.year as MY, file.mtime.month as MM, file.mtime.day as MD
from #src/pod-🎧 
WHERE file.name != "Template Podcast"
sort file.ctime asc
``` 
### Videos
```dataview 
table file.mtime.year as MY, file.mtime.month as MM, file.mtime.day as MD
from #src/vid-🎥 AND  !#trading 
WHERE file.name != "Template Youtube"
sort file.ctime asc
```
### Meet-up
```dataview 
table file.mtime.year as MY, file.mtime.month as MM, file.mtime.day as MD
from #src/discu-🍻 
WHERE file.name != "Template Discussion"
sort file.ctime asc
``` 
### Thoughts
```dataview 
table file.mtime.year as MY, file.mtime.month as MM, file.mtime.day as MD
from #src/thoughts-💭 
WHERE file.name != "Template Ideas"
sort file.ctime asc
``` 
 > [!summary] 
 > ```dataview 
table Author, M_Topics,Publish_Date,Reviewed_Date, Note, Status
from #🧠/📥/📚 OR #📈/📥/📚 AND !#⚙️
sort file.ctime asc


# Trading
## - 🌱️
```dataview 
table file.mtime.year as MY, file.mtime.month as MM, file.mtime.day as MD, Status
from  !#🧠/🗺️ 
WHERE type = "Note-📝" AND Related_Notes = [[Trading MOC]]
sort file.ctime asc
``` 

## - 🌿️
```dataview 
table file.mtime.year as MY, file.mtime.month as MM, file.mtime.day as MD
from #📈/📥/📝/🌿   AND !#🧠/🗺️ 
sort file.ctime asc
``` 

## - 🌞️
```dataview 
table year
from #📈/📥/🍻/🟥 
``` 


```dataview 
table file.mtime.year as MY, file.mtime.month as MM, file.mtime.day as MD, Status
from [[Meditation]]
sort file.ctime asc
``` 

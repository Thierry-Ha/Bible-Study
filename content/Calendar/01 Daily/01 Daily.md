## Daily Journal
```dataview
table WITHOUT ID
	link(file.name) as "Day",
	focus as "Focus"
from #Trading/Journal/d 
WHERE file.name != "Template Journal Trading"
LIMIT 7
```
## Weekly:
```dataview
table WITHOUT ID
	link(file.name) as "Week",
	focus as "Focus"
from #Trading/Journal/w
WHERE file.name != "Weekly Trading Journal"
LIMIT 2
```

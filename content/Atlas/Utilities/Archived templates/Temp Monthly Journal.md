---
month: <% tp.date.now("MM", 0, tp.file.title, "YYYY--WW") %>-<% tp.date.now("MMM", 0, tp.file.title, "gggg-[W]ww") %>
year: <% tp.date.now("YYYY", 0, tp.file.title, "gggg-[W]ww") %>
banner: "https://preview.redd.it/arqa352ph7x61.jpg?width=960&crop=smart&auto=webp&s=84f9245d607b029667d5bfc4abf36547fc6213de"
---
⠀
###### [[<% tp.date.now("YYYY - MM-MMMM", "P-1M", tp.file.title, "YYYY - MM-MMMM") %>|↶ PREVIOUS MONTH]] ⁝ [[<% tp.date.now("YYYY - MM-MMMM", "P1M", tp.file.title, "YYYY - MM-MMMM") %>|FOLLOWING MONTH ↷]]
# ◌ <% tp.file.title %>

## Weeks
```dataview
TABLE
month as "Month"
FROM #Journal/w
WHERE month = "<% tp.file.title %>"
```

## Days
```dataview
TABLE WITHOUT ID
	link(file.name) as "Day",
	wake-early AS "🌄",
	posture AS "Posture",
	meditate AS "🧘",
	abs AS "🍫",
	cold-shower AS "🥶",
	Worktime AS "Work",
	exercise AS "🏃‍♂️",
	daily-rd AS "R&D",
	streching AS "Strech",
	followed-the-rules AS "⚖️",
	journal-and-plan-next-day AS "📝"
	FROM #Journal/d
	SORT file.name DESC
	LIMIT 30
WHERE file.name != "Temp Daily Journal"
WHERE month = "<% tp.file.title %>"
```

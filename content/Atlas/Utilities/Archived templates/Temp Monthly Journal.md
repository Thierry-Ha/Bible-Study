---
month: 01-Aug
year: 0007
banner: "https://preview.redd.it/arqa352ph7x61.jpg?width=960&crop=smart&auto=webp&s=84f9245d607b029667d5bfc4abf36547fc6213de"
---
⠀
###### [[0006 - 12-December|↶ PREVIOUS MONTH]] ⁝ [[0007 - 02-February|FOLLOWING MONTH ↷]]
# ◌ JBP - Genesis - Lecture 7

## Weeks
```dataview
TABLE
month as "Month"
FROM #Journal/w
WHERE month = "JBP - Genesis - Lecture 7"
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
WHERE month = "JBP - Genesis - Lecture 7"
```

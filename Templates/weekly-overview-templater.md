---
title: <% tp.file.title %>
created: <% tp.file.creation_date() %>
tags:
  - "#Journal"
  - weekly
---
# <% moment(tp.file.title).startOf("week").format("MMM DD") %> - <% moment(tp.file.title).endOf("week").format("MMM DD") %>

[[Journal/Weekly/<% moment(tp.file.title).subtract(1, "week").format("gggg-[W]ww") %> | :luc_chevrons_left: Previous Week]] |[[Journal/Weekly/<% moment(tp.file.title).add(1, "week").format("gggg-[W]ww") %> | Next Week :luc_chevrons_right: ]]

| [[Journal/Daily/<% moment(tp.file.title).startOf("week").add(0, "day").format("MM-MMMM") %>/<% moment(tp.file.title).startOf("week").add(0, "day").format("YYYY-MM-DD") %> \| Sunday]] | [[Journal/Daily/<% moment(tp.file.title).startOf("week").add(1, "day").format("MM-MMMM") %>/<% moment(tp.file.title).startOf("week").add(1, "day").format("YYYY-MM-DD") %> \| Monday]] | [[Journal/Daily/<% moment(tp.file.title).startOf("week").add(20, "day").format("MM-MMMM") %>/<% moment(tp.file.title).startOf("week").add(2, "day").format("YYYY-MM-DD") %> \| Tuesday]] | [[Journal/Daily/<% moment(tp.file.title).startOf("week").add(3, "day").format("MM-MMMM") %>/<% moment(tp.file.title).startOf("week").add(3, "day").format("YYYY-MM-DD") %> \| Wednesday]] | [[Journal/Daily/<% moment(tp.file.title).startOf("week").add(4, "day").format("MM-MMMM") %>/<% moment(tp.file.title).startOf("week").add(4, "day").format("YYYY-MM-DD") %> \| Thursday]] | [[Journal/Daily/<% moment(tp.file.title).startOf("week").add(5, "day").format("MM-MMMM") %>/<% moment(tp.file.title).startOf("week").add(5, "day").format("YYYY-MM-DD") %> \| Friday]] | [[Journal/Daily/<% moment(tp.file.title).startOf("week").add(6, "day").format("MM-MMMM") %>/<% moment(tp.file.title).startOf("week").add(6, "day").format("YYYY-MM-DD") %> \| Saturday]] |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

---
## Habit Tracker of <% tp.file.title %>

```dataview
table without id
	file.link AS Date,
	weight AS "📉",
	bpm_avg AS "💗",
	sleep AS "💤",
	steps AS "👟",
	distance AS "📍",
	choice(vitamins, "✅", "❌") AS "💊",
	choice(move_goal, "✅", "❌") AS "🚶‍♂️",
	choice(exercise_goal, "✅", "❌") AS "🏃‍♂️",
	choice(stand_goal, "✅", "❌") AS "🧍‍♂️"
from #daily
where this.file.name = week_num
sort file.name ASC
```

---
## Primary Goals

- [ ] 

---
## Secondary Goals

- [ ] 

---
### NOTES

- 
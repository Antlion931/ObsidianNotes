# Daily notes

```dataviewjs
const calendarData = {
colors: {
red: ["#ff9e82","#ff7b55","#ff4d1a","#e73400","#bd2a00",]
},
entries: []
}

for(let page of dv.pages('"Daily notes"').where(p=>p["Daily notes"])){
calendarData.entries.push({
date: page.file.name,
intensity: page.Exercise,
content: await dv.span(`[](${page.file.name})`), //for hover preview
})

}

renderHeatmapCalendar(this.container, calendarData)

```
# Workout

```dataviewjs
const calendarData = {
colors: {
red: ["#ff9e82","#ff7b55","#ff4d1a","#e73400","#bd2a00",]
},
entries: []
}

for(let page of dv.pages('"Daily notes"').where(p=>p["Workout"])){
calendarData.entries.push({
date: page.file.name,
intensity: page.Exercise,
content: await dv.span(`[](${page.file.name})`), //for hover preview
})

}

renderHeatmapCalendar(this.container, calendarData)

```

# English

```dataviewjs
const calendarData = {
colors: {
red: ["#ff9e82","#ff7b55","#ff4d1a","#e73400","#bd2a00",]
},
entries: []
}

for(let page of dv.pages('"Daily notes"').where(p=>p["English"])){
calendarData.entries.push({
date: page.file.name,
intensity: page.Exercise,
content: await dv.span(`[](${page.file.name})`), //for hover preview
})

}

renderHeatmapCalendar(this.container, calendarData)

```

#### Translations to make

```dataview
TASK WHERE contains(tags, "#translateLater") GROUP BY file.link
```

# Path to cybersecuirty expert

```dataviewjs
const calendarData = {
colors: {
red: ["#ff9e82","#ff7b55","#ff4d1a","#e73400","#bd2a00",]
},
entries: []
}

for(let page of dv.pages('"Daily notes"').where(p=>p["Path to cybersecurity expert"])){
calendarData.entries.push({
date: page.file.name,
intensity: page.Exercise,
content: await dv.span(`[](${page.file.name})`), //for hover preview
})

}

renderHeatmapCalendar(this.container, calendarData)
```

#### Things to work on

```dataview
TASK WHERE contains(tags, "#todo") AND contains(file.tags, "#cybersecurity") GROUP BY file.link
```

# Algebra

```dataviewjs
const calendarData = {
colors: {
red: ["#ff9e82","#ff7b55","#ff4d1a","#e73400","#bd2a00",]
},
entries: []
}

for(let page of dv.pages('"Daily notes"').where(p=>p["Algebra"])){
calendarData.entries.push({
date: page.file.name,
intensity: page.Exercise,
content: await dv.span(`[](${page.file.name})`), //for hover preview
})

}

renderHeatmapCalendar(this.container, calendarData)
```

#### Things to work on

```dataview
TASK WHERE contains(tags, "#todo") AND contains(file.tags, "#algebra") AND contains(file.tags, "#pwr") GROUP BY file.link
```
# Cybersecurity

```dataviewjs
const calendarData = {
colors: {
red: ["#ff9e82","#ff7b55","#ff4d1a","#e73400","#bd2a00",]
},
entries: []
}

for(let page of dv.pages('"Daily notes"').where(p=>p["Cybersecurity"])){
calendarData.entries.push({
date: page.file.name,
intensity: page.Exercise,
content: await dv.span(`[](${page.file.name})`), //for hover preview
})

}

renderHeatmapCalendar(this.container, calendarData)
```

#### Things to work on

```dataview
TASK WHERE contains(tags, "#todo") AND contains(file.tags, "#cybersecurity") AND contains(file.tags, "#pwr") GROUP BY file.link
```
# Embedded systems

```dataviewjs

const calendarData = {
colors: {
red: ["#ff9e82","#ff7b55","#ff4d1a","#e73400","#bd2a00",]
},
entries: []
}

for(let page of dv.pages('"Daily notes"').where(p=>p["Embedded system"])){
calendarData.entries.push({
date: page.file.name,
intensity: page.Exercise,
content: await dv.span(`[](${page.file.name})`), //for hover preview
})

}

renderHeatmapCalendar(this.container, calendarData)
```

#### Things to work on

```dataview
TASK WHERE contains(tags, "#todo") AND contains(file.tags, "#embedded") AND contains(file.tags, "#pwr") GROUP BY file.link
```
# Theoretical informatics

```dataviewjs

const calendarData = {
colors: {
red: ["#ff9e82","#ff7b55","#ff4d1a","#e73400","#bd2a00",]
},
entries: []
}

for(let page of dv.pages('"Daily notes"').where(p=>p["Theoretical informatics"])){
calendarData.entries.push({
date: page.file.name,
intensity: page.Exercise,
content: await dv.span(`[](${page.file.name})`), //for hover preview
})

}

renderHeatmapCalendar(this.container, calendarData)
```

#### Things to work on

```dataview
TASK WHERE contains(tags, "#todo") AND contains(file.tags, "#theoreticalInformatics") AND contains(file.tags, "#pwr") GROUP BY file.link
```

# Programming challenges

```dataviewjs

const calendarData = {
colors: {
red: ["#ff9e82","#ff7b55","#ff4d1a","#e73400","#bd2a00",]
},
entries: []
}

for(let page of dv.pages('"Daily notes"').where(p=>p["Programming challenges"])){
calendarData.entries.push({
date: page.file.name,
intensity: page.Exercise,
content: await dv.span(`[](${page.file.name})`), //for hover preview
})

}

renderHeatmapCalendar(this.container, calendarData)
```

#### Things to work on

```dataview
TASK WHERE contains(tags, "#todo") AND contains(file.tags, "#programmingChallenges") GROUP BY file.link
```

# Book

```dataviewjs

const calendarData = {
colors: {
red: ["#ff9e82","#ff7b55","#ff4d1a","#e73400","#bd2a00",]
},
entries: []
}

for(let page of dv.pages('"Daily notes"').where(p=>p["Book"])){
calendarData.entries.push({
date: page.file.name,
intensity: page.Exercise,
content: await dv.span(`[](${page.file.name})`), //for hover preview
})

}

renderHeatmapCalendar(this.container, calendarData)
```

#### Things to work on

```dataview
TASK WHERE contains(tags, "#todo") AND contains(file.tags, "#book") GROUP BY file.link
```
# Programming paradigms 

```dataviewjs

const calendarData = {
colors: {
red: ["#ff9e82","#ff7b55","#ff4d1a","#e73400","#bd2a00",]
},
entries: []
}

for(let page of dv.pages('"Daily notes"').where(p=>p["Programming paradigms"])){
calendarData.entries.push({
date: page.file.name,
intensity: page.Exercise,
content: await dv.span(`[](${page.file.name})`), //for hover preview
})

}

renderHeatmapCalendar(this.container, calendarData)
```

#### Things to work on

```dataview
TASK WHERE contains(tags, "#todo") AND contains(file.tags, "#Programming paradigms") GROUP BY file.link
```
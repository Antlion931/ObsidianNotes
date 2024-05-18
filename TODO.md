
```dataviewjs
const calendarData = {
    color: "default",
    entries: []
}

function add_them(p) {
    let list = ["English", "Algebra", "Path to cybersecurity expert",
    "Cybersecurity", "Embedded systems", "Theoretical informatics", "Programming challenges", "Book", "Programming paradigms"];
    let sum = 0;

    for (let l of list) {
        if (typeof p[l] !== 'undefined') {
            sum += p[l];
        }
    }
    
    return sum;
}

for(let page of dv.pages('"Daily notes"').where(p=>add_them(p))){
    calendarData.entries.push({
    date: page.file.name,
    intensity: add_them(page),
    content: await dv.span(`[](${page.file.name})`), //for hover preview
})

}

renderHeatmapCalendar(this.container, calendarData)
```

# Workout

```dataviewjs
const calendarData = {
    color: "default",
    entries: []
}

function add_them(p) {
    let list = ["Workout"];
    let sum = 0;

    for (let l of list) {
        if (typeof p[l] !== 'undefined') {
            sum += p[l];
        }
    }
    
    return sum;
}

for(let page of dv.pages('"Daily notes"').where(p=>add_them(p))){
    calendarData.entries.push({
    date: page.file.name,
    intensity: add_them(page),
    content: await dv.span(`[](${page.file.name})`), //for hover preview
})

}

renderHeatmapCalendar(this.container, calendarData)
```

# English

```dataviewjs
const calendarData = {
    color: "default",
    entries: []
}

function add_them(p) {
    let list = ["English"];
    let sum = 0;

    for (let l of list) {
        if (typeof p[l] !== 'undefined') {
            sum += p[l];
        }
    }
    
    return sum;
}

for(let page of dv.pages('"Daily notes"').where(p=>add_them(p))){
    calendarData.entries.push({
    date: page.file.name,
    intensity: add_them(page),
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
    color: "default",
    entries: []
}

function add_them(p) {
    let list = ["Path to cybersecurity expert"];
    let sum = 0;

    for (let l of list) {
        if (typeof p[l] !== 'undefined') {
            sum += p[l];
        }
    }
    
    return sum;
}

for(let page of dv.pages('"Daily notes"').where(p=>add_them(p))){
    calendarData.entries.push({
    date: page.file.name,
    intensity: add_them(page),
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
    color: "default",
    entries: []
}

function add_them(p) {
    let list = ["Algebra"];
    let sum = 0;

    for (let l of list) {
        if (typeof p[l] !== 'undefined') {
            sum += p[l];
        }
    }
    
    return sum;
}

for(let page of dv.pages('"Daily notes"').where(p=>add_them(p))){
    calendarData.entries.push({
    date: page.file.name,
    intensity: add_them(page),
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
    color: "default",
    entries: []
}

function add_them(p) {
    let list = ["Cybersecurity"];
    let sum = 0;

    for (let l of list) {
        if (typeof p[l] !== 'undefined') {
            sum += p[l];
        }
    }
    
    return sum;
}

for(let page of dv.pages('"Daily notes"').where(p=>add_them(p))){
    calendarData.entries.push({
    date: page.file.name,
    intensity: add_them(page),
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
    color: "default",
    entries: []
}

function add_them(p) {
    let list = ["Embedded systems"];
    let sum = 0;

    for (let l of list) {
        if (typeof p[l] !== 'undefined') {
            sum += p[l];
        }
    }
    
    return sum;
}

for(let page of dv.pages('"Daily notes"').where(p=>add_them(p))){
    calendarData.entries.push({
    date: page.file.name,
    intensity: add_them(page),
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
    color: "default",
    entries: []
}

function add_them(p) {
    let list = ["Theoretical informatics"];
    let sum = 0;

    for (let l of list) {
        if (typeof p[l] !== 'undefined') {
            sum += p[l];
        }
    }
    
    return sum;
}

for(let page of dv.pages('"Daily notes"').where(p=>add_them(p))){
    calendarData.entries.push({
    date: page.file.name,
    intensity: add_them(page),
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
    color: "default",
    entries: []
}

function add_them(p) {
    let list = ["Programming challenges"];
    let sum = 0;

    for (let l of list) {
        if (typeof p[l] !== 'undefined') {
            sum += p[l];
        }
    }
    
    return sum;
}

for(let page of dv.pages('"Daily notes"').where(p=>add_them(p))){
    calendarData.entries.push({
    date: page.file.name,
    intensity: add_them(page),
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
    color: "default",
    entries: []
}

function add_them(p) {
    let list = ["Book"];
    let sum = 0;

    for (let l of list) {
        if (typeof p[l] !== 'undefined') {
            sum += p[l];
        }
    }
    
    return sum;
}

for(let page of dv.pages('"Daily notes"').where(p=>add_them(p))){
    calendarData.entries.push({
    date: page.file.name,
    intensity: add_them(page),
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
    color: "default",
    entries: []
}

function add_them(p) {
    let list = ["Programming paradigms"];
    let sum = 0;

    for (let l of list) {
        if (typeof p[l] !== 'undefined') {
            sum += p[l];
        }
    }
    
    return sum;
}

for(let page of dv.pages('"Daily notes"').where(p=>add_them(p))){
    calendarData.entries.push({
    date: page.file.name,
    intensity: add_them(page),
    content: await dv.span(`[](${page.file.name})`), //for hover preview
})

}

renderHeatmapCalendar(this.container, calendarData)
```

#### Things to work on

```dataview
TASK WHERE contains(tags, "#todo") AND contains(file.tags, "#programmingParadigms") AND contains(file.tags, "#pwr") GROUP BY file.link
```
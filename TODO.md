
```dataviewjs
const calendarData = {
    color: "default",
    entries: []
}

function add_them(p) {
    let list = ["English", "Algebra", "Path to cybersecurity expert",
    "Cybersecurity", "Embedded systems", "Theoretical informatics", "Programming challenges", "Book", "Programming paradigms", "CV"];
    let sum = 0;

    for (let l of list) {
        //dv.span("<br>" + p[l]) // uncomment for troubleshooting
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

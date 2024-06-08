
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

# CV

- [x] Change mail to some that looks more like your name and surname without numbers
- [x] Change colouring to some that is more light
- [ ] In Links add phone number, github, Linkedin, Github and Youtube and make sure that all of them are in good quality, Changeg name to some that is more fitting
- [x] In Education name of a University should be less visible and my major should be more
- [x] In Education add a little description of my studies
- [x] Under my name up the top add a little text, some called cover letter, it should be written for every job.
- [x] Change English to B2
- [x] Different pattern for GDPR
- [x] In Interests be more thorough, like write about arranging MTG tournaments and Reading books of Brandon Sanderson, and a little bit about them
- [x] The main part should be totaly changed, focuse on specific project and technologies that are used in them, You need to go pass through Bot, Key words are important. For sure add Lovetrain, and 2 more depending on Job.
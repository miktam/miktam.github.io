---
layout: post
title: "Sorting Arrays in Javascript"
date: 2014-07-12
---
### Example
```
    [
      {name: 'Dominika',age: 2},
      {name: 'Lilia',   age: 31},
      {name: 'Andrei',  age: 32},
      {name: 'Jan',     age: 6}
    ].sort((a, b) => {
      return a.age - b.age;
    })
```
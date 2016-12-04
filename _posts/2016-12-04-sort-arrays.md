---
layout: post
title: "Sorting Arrays in ES6"
date: 2016-12-04
---
### Sort array by attribute in ES6
{% highlight javascript %}
 [
  {name: 'Dominika',age: 2},
  {name: 'Lilia',   age: 31},
  {name: 'Andrei',  age: 32},
  {name: 'Jan',     age: 6}
 ].sort((a, b) => a.age - b.age)
 /* will print
 [ { name: 'Dominika', age: 2 },
   { name: 'Jan', age: 6 },
   { name: 'Lilia', age: 31 },
   { name: 'Andrei', age: 32 } ]
 */
{% endhighlight %}
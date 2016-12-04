---
layout: post
title: "Sorting Array by Attribute in ES6"
date: 2016-12-04
---
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

### Why?
- [Array.sort](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort)
- [Implicit return in consise function body](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions#Function_body)

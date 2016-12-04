---
layout: post
title: "Binding in Javascript"
date: 2014-08-10
---
### Must read
* [Getting Out of Binding Situations in JavaScript](http://alistapart.com/article/getoutbindingsituations) by Christophe Porteneuve
* [Function.prototype.bind definition](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/bind?redirectlocale=en-US&redirectslug=JavaScript%2FReference%2FGlobal_Objects%2FFunction%2Fbind)

### Example
```
const x = 9; 
const module = {
  x: 81,
  getX: () => { return this.x; }
};

module.getX(); // 81

const getX = module.getX;
getX(); // 9, because in this case, "this" refers to the global object

// create a new function with 'this' bound to module
const boundGetX = getX.bind(module);
boundGetX(); // 81
```
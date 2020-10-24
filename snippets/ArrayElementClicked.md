---
title: ArrayElementClicked
tags: Array, Intermediate, DOM
---

Logs an element inside an array that was clicked. Only works as a result of user 
action (specifically the "click" event listener).

- Iterates over a given array using `Array.prototype.forEach()`
- Adds an event listener to each item `target.addEventListener("click", function);`
- Console Logs the clicked element

```js
function ArrayElementClicked(arr){
  arr.forEach( element => {
    element.addEventListener("click", () => console.log(element))
  })
}
```

```js
const items = document.querySelectorAll("li");
ArrayElementClicked(items); // '<li>Second Item</li>'
```

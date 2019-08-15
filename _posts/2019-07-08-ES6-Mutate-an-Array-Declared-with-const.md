---
layout: default
title: ES6: Mutate an Array Declared with const
---
const s = [5, 7, 2];
function editInPlace() {
  "use strict";
  // change code below this line
  s.sort(function(a, b){return a - b});
  // change code above this line
}
editInPlace();
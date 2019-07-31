---
layout: default
title: Write Higher Order Arrow Functions
---
const realNumberArray = [4, 5.6, -9.8, 3.14, 42, 6, 8.34, -2];
const squareList = (arr) => {
  "use strict";
  // change code below this line: filter function selects only values that match its function argument; map function applies its function argument to the values of the array
  const squaredIntegers = arr.filter(x => x > 0 && x % parseInt(x) === 0 ).map(x => x * x);
  // change code above this line
  return squaredIntegers;
};
// test your code
const squaredIntegers = squareList(realNumberArray);
console.log(squaredIntegers);
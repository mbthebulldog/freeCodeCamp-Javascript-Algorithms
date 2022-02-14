---
layout: default
title: Functional Programming: Use Higher-Order Functions map, filter, or reduce to Solve a Complex Problem
---
const squareList = arr => {
  // Only change code below this line
  return arr.filter(num => num % 1 === 0 && num > 0).map(num => num * num);
  // Only change code above this line
};

const squaredIntegers = squareList([-3, 4.8, 5, 3, -3.2]);
console.log(squaredIntegers);
---
layout: default
title: Basic JavaScript: Using Recursion To Create A Range Of Numbers
---
function rangeOfNumbers(startNum, endNum) {
  if (startNum === endNum) {
    return [endNum];
  } else {
    var numbers = rangeOfNumbers(startNum, endNum - 1);
    numbers.push(endNum);
    return numbers;
  }
};
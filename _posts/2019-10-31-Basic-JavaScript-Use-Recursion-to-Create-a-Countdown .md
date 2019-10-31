---
layout: default
title: Basic JavaScript: Use Recursion to Create a Countdown
---
//Only change code below this line
function countdown(myArray, n){
  if (n <= 0) {
    return myArray;
  } else {
    myArray.push(n);
    countdown(myArray, n-1);
  }
}
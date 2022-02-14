---
layout: default
title: Functional Programming: Sum All Numbers in a Range
---
function sumAll(arr) {
  
  //sort the array
  function compareNumbers(a, b) {
    return a - b;
  }
  arr.sort(compareNumbers);
  
  //set variables
  let a = arr[0];
  let b = arr[1];
  let range = b - a + 1;
  
  //calculate the sumtorial using sum of continuous range formula
  return (a + b) * range / 2;

  //log the sorted array and the sumtorial results
  return sum;
}

sumAll([1, 4]);
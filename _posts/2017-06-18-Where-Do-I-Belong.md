---
layout: default
title: Where Do I Belong?
---
function getIndexToIns(arr, num) {
  arr.push(num); //adds the new number to the array
  arr.sort(function(a, b){return a-b;}); //sorts the array from smallest to largest
  
  for (var i = 0; i < arr.length ; i++) { //I just love me some for loops
    if (arr[i] === num) { //returns the first index boasting that new number in our now-sorted array
       return i;
    }
  }
}

getIndexToIns([2, 5, 10], 15);

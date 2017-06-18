---
layout: default
title: Seek and Destroy
---
function destroyer(arr) {
  var deletors = Array.prototype.slice.call(arguments, 1); //gets elimination values from the arguments (by slicing AFTER arguments[0], which is arr)

  var clean = arr.filter(function(killer) { //filter out elements matching deletors
    if (deletors.indexOf(killer) === -1) {
      return true;
    } //whenever indexOf returns -1, meaning that value of arr was not found in deletors, then we return true to preserve it
  });
  return clean;
}

destroyer([1, 2, 3, 1, 2, 3], 2, 3);

/*function destroyer(arr, val1, val2, val3) {
  return arr.filter(function(item) {    
    return !(item === val1 || item === val2 || item === val3);    
  });
}

destroyer([1, 2, 3, 1, 2, 3], 2, 3);*/
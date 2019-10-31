---
layout: default
title: Basic Algorithm Scripting: Falsy Bouncer
---
function bouncer(arr) {
    return arr.filter(Boolean);
} //simply use the Boolean function to filter out all falsy values

bouncer([6, "and", "", false, 20, "blackbirds"]);


OR

function bouncer(arr) {
  let newArr = [];
  for (let i = 0; i < arr.length; i++) {
    if (arr[i]) {
      newArr.push(arr[i]);
    }
  }
  return newArr;
}

bouncer([7, "ate", "", false, 9]);
---
layout: default
title: Basic Algorithm Scripting: Repeat a String Repeat a String
---
function repeatStringNumTimes(str, num) {
  var long = '';
  
  for (var i = 0; i < num; i++) { //repeat loop a specific number of times according to num
    long = long.concat(str); //add the contents of str to long once each loopthrough
  }  
  return long;
}

repeatStringNumTimes("abc", 3);

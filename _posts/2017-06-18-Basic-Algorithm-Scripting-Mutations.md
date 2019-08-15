---
layout: default
title: Basic Algorithm Scripting: Mutations
---
function mutation(arr) {
  
  var first = arr[0].toLowerCase(); //separate the two words into distinct, all-lowercase variables
  var second = arr[1].toLowerCase(); //
  answer = true; //create a boolean variable
  
  for (var i = 0; i < second.length ; i++) { //iterate through every letter of the second word
    
    if (first.indexOf(second[i]) == -1) {
      answer = false;
    } //if indexOf cannot find a matching letter in the first word for any letter of the second word, it will set answer to false
  
  }
  
  return answer;
}

mutation(["bonjour, senorita princesa", "sup"]);

---
layout: default
title: Basic Algorithm Scripting: Confirm the Ending
---
function confirmEnding(str, target) {
  str = str.substr(str.length - target.length, target.length); //delete all but the last letter of the string
  return str == target; //compare last letter of string to target letter
}

confirmEnding("Hickorydickorydock", "n");

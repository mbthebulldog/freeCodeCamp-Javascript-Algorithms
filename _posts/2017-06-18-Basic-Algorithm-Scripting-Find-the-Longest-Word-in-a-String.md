---
layout: default
title: Basic Algorithm Scripting: Find the Longest Word in a String
---
function findLongestWord(str) {
  str = str.split(/\s/g); //split the string at every space
  var longest = 0;
  for (var i = 0; i < str.length; i++) {
    longest = longest < str[i].length ? str[i].length : longest;
  } //ternary operator assigns the value of the i-th element of the string iff it is the largest number so far
  return longest;
}

findLongestWord("The longest word I know is 'pneumonoultramicroscopicsilicovolcanoconiosis'. Those poor, poor Pompeii…-ites(?).");

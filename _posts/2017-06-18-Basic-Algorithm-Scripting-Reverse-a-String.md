---
layout: default
title: Basic Algorithm Scripting: Reverse a String
---
function reverseString(str) {
  return str.split("").reverse().join(""); //splits, reverses, and joins the string together in one line
}

reverseString("Coding is quite fun!");

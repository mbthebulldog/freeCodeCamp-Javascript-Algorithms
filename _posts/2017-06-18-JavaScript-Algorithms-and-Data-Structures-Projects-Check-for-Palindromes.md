---
layout: default
title: JavaScript Algorithms and Data Structures Projects: Check for Palindromes
---
function palindrome(str) {
  str = str.toLowerCase().replace(/[\W_]/g, '');  //makes all uppercase letters lowercase and eliminates all non-letters
  return str === str.split('').reverse().join(''); //returns true if the string is the same as its reversed self
}

palindrome("zu*p@*p_a");



/*  return fore = str.replace(/[^\w\d]/g, ''); 
  back = str.split('').reverse().join('');
  
 
  return fore==back;*/

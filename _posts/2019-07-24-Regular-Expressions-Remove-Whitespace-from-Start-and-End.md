---
layout: default
title: Regular Expressions: Remove Whitespace from Start and End
---
let hello = "   Hello, World!  ";
let wsRegex = /^\s+|\s+$/g; // Change this line
let result = hello.replace(wsRegex, ""); // Change this line
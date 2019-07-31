---
layout: default
title: Regular Expressions: Restrict Possible Usernames
---
let username = "JackOfAllTrades";
let userCheck = /^[a-z]{2,}\d*$/i; // Change this line
let result = userCheck.test(username);
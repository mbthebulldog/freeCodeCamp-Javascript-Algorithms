---
layout: default
title: Search and Replace
---
function myReplace(str, before, after) {
  if (before.charAt(0) === before.charAt(0).toUpperCase()) {
    after = after.replace(after.charAt(0), after.charAt(0).toUpperCase())
  } else if (before.charAt(0) === before.charAt(0).toLowerCase()) {
    after = after.replace(after.charAt(0), after.charAt(0).toLowerCase())
  }

  str = str.replace(before, after);
  return str;
}

myReplace("A quick brown fox jumped over the lazy dog", "jumped", "leaped");
---
layout: default
title: Truncate a String
---
function truncateString(str, num) {
  
  if (str.length > num) { //if str < num, simply return str
    
    if (num <= 3) {
      str = str.slice(0, num);
      str = str.concat('...');
    } //if str < 3, truncate and add ellipsis
    else {
    str = str.slice(0, num - 3);
    str = str.concat('...');
    } //if str > 3 (but still < num), truncate 3 extra slots to make room for the ellipsis
  }
  return str;
}

truncateString("Abs-tisket a-tasket A green and yellow basketball", 2);

---
layout: default
title: Title Case a Sentence
---
function titleCase(str) {
  str = str.toLowerCase(); //first step: make all the letters lowercase
  str = str.split(/\s/g); //next, split into words
  
  for (var i = 0; i < str.length ; i++) {
    str[i] = str[i].split(''); //seperate the word
    str[i][0] = str[i][0].toUpperCase(); //make the first letter capital
    str[i] = str[i].join(''); //join the word together again
  }
  
  str = str.join(' '); //join the string together again
  return str;
}

titleCase("I'm a big fat tea pot, baby.");

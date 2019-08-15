---
layout: default
title: Basic Data Structures: Check if an Object has a Property
---
let users = {
  Alan: {
    age: 27,
    online: true
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: true
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function isEveryoneHere(obj) {
  // change code below this line
  return 'Alan' in users && 'Jeff' in users && 'Sarah' in users && 'Ryan' in users;
  // change code above this line
}

console.log(isEveryoneHere(users));
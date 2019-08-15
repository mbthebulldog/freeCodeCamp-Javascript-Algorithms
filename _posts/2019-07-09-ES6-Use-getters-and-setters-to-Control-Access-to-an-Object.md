---
layout: default
title: ES6: Use getters and setters to Control Access to an Object
---
function makeClass() {
  "use strict";
  /* Alter code below this line */
  class Thermostat {
    constructor(temperature) {
      this.temperature = temperature;
    }
    get celsius(){
      return 5/9 * (this.temperature - 32);
    }
    set celsius(x) {
      this.temperature = x * 9.0 / 5 + 32;
    }
  }
  /* Alter code above this line */
  return Thermostat;
}
const Thermostat = makeClass();
const thermos = new Thermostat(76); // setting in Fahrenheit scale
let temp = thermos.temperature; // 24.44 in C
thermos.temperature = 26;
temp = thermos.temperature; // 26 in C
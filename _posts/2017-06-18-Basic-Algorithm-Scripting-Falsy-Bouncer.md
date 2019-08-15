---
layout: default
title: Basic Algorithm Scripting: Falsy Bouncer
---
function bouncer(arr) {
    return arr.filter(Boolean);
} //simply use the Boolean function to filter out all falsy values

bouncer([6, "and", "", false, 20, "blackbirds"]);

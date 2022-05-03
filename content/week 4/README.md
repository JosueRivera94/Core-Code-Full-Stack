# Week 4 : React & Node
---
## 📖 Week challenges (Monday)

### 1.Two To One
``` javascript
function longest(s1, s2) {
  let a = [... new Set(s1.split(""))];
  let b = [... new Set(s2.split(""))];

  for (let i=0; i<b.length; i++){
  	a.push(b[i]);
  }
  let init_combo = [... new Set(a)];
  let combo = init_combo.sort().join("");

  return combo;
}
```
## 📖 Week challenges (Tuesday)

### 1.Leap Years
``` javascript
function isLeapYear(year) {
  return (year % 100 !== 0 && year % 4 === 0) || year % 400 === 0;
}
```
## 📖 Week challenges (Wednesday)

### 1.Maximum Length Difference
``` javascript
function mxdiflg(a1, a2) {
    if (a1.length === 0 || a2.length === 0) return -1

  const length1 = a1.map(string => string.length)
  const length2 = a2.map(string => string.length)

  return Math.max(
    Math.max(...length1) - Math.min(...length2),
    Math.max(...length2) - Math.min(...length1)
  )
}
```
## 📖 Week challenges (Thursday)

### 1.Base64 Numeric Translator 
``` javascript

```




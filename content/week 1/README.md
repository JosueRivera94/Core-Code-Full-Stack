
# Week 1 : Warm up Javascript exercises before React exercises
---
## 📖 Week challenges (Tuesday)

### 1.Ensure question
``` javascript
function ensureQuestion(s) {
  return /\?$/.test(s) ? s : s+'?'
}
```
### 2.Ensure question
``` javascript
function reverseWords(str){
 return str.split(' ').reverse().join(' ');
}
```
## 📖 Week challenges (wednesday)

### 1.Find the smallest integer in the array
``` javascript
class SmallestIntegerFinder {
  findSmallestInt(args) {
     return Math.min(...args)
  }
}
```
## 📖 Week challenges (Thursday)

### 1.Odd or Even
``` javascript
function oddOrEven(array) {
   let sum = 0;
  
  if (array.length !== 0) {
    sum = array.reduce((x, y) => x + y);
    return sum % 2 === 0 ? 'even' : 'odd';
    
  } else {
    return 'even';
  }
}
```

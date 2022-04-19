# Week 2 : Front End
---

### 1. Palindrome Strings
``` javascript
function isPalindrome(line) {
   return (''+line) === (''+line).split('').reverse().join('');
}
```
### 2. Multiple of Index
``` javascript
function multipleOfIndex(array) {
  return array.filter((num, i) => num % i === 0);
}
```

### 3. Well of Ideas
``` javascript
function well(x){
const count = x.reduce((s, v) => s + (v == 'good'), 0);
  return count ? count > 2 ? 'I smell a series!' : 'Publish!' : 'Fail!';
}
```

### 4. Decode the Morse code
``` javascript
decodeMorse = function(morseCode){
morseCode = morseCode.trim();
  let refinedData = morseCode.split('   ');
  let result = [];
  
  for (let i = 0; i < refinedData.length; i++) {
    let temp = refinedData[i].split(' ');
    for (let j = 0; j < temp.length; j++) {
      if (MORSE_CODE[temp[j]]) {
        result.push(MORSE_CODE[temp[j]]);
      }
    }
    
    if (i !== refinedData.length - 1) {
    result.push(' ');
    }
  }
  return result.join('');
}
```


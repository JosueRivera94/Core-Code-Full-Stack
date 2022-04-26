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

### 5. React Santa Wish List
``` javascript
const React = require("react");

class WishlistForm extends React.Component {
  constructor(props) {
    super(props);
    this.state = { name: '', wish: '', priority: 1 };
    this.handleNameChange = this.handleNameChange.bind(this);
    this.handleWishChange = this.handleWishChange.bind(this);
    this.handlePriorityChange = this.handlePriorityChange.bind(this);
    this.handleSubmit = this.handleSubmit.bind(this);
  }
  
  handleNameChange(e) {
    this.setState({name: e.target.value});
  }
  
  handleWishChange(e) {
    this.setState({wish: e.target.value});
  }
  
  
  handlePriorityChange(e) {
    this.setState({priority: e.target.value});
  }
  
  handleSubmit(e){
    e.preventDefault();
    this.props.send(this.state);
  }
  render() {
    return (
      <form onSubmit={this.handleSubmit}>
       Name: <input type="text" id="name" value={this.state.name} onChange={this.handleNameChange}/>
       Wish: <textarea rows="10" cols="10" id="wish" value={this.state.wish} onChange={this.handleWishChange} />
       <br />
       Wish Priority:
       <select value={this.state.priority} id="priority" onChange={this.handlePriorityChange}>
         <option value={1}>1</option>
         <option value={2}>2</option>
         <option value={3}>3</option>
         <option value={4}>4</option>
         <option value={5}>5</option>
      </select>
      </form>
    );
  }
};
```


1. ## Valid Parentheses exercise

```javascript
function validParentheses(parens) {
    // your code here ..
    let count = 0;
    for (let i = 0; i < parens.length; i++) {
        if (parens[i] == '(') {
            count += 1
        } else {
            count -= 1
        }
        if (count < 0) return false;
    }
    return count == 0;
}
```
2. ## onvert String To Camel Case exercise
```javascript
function toCamelCase(str){
  let newStr = "";
  if(str){
    let wordArr = str.split(/[-_]/g);
    for (let i in wordArr){
      if(i > 0){
        newStr += wordArr[i].charAt(0).toUpperCase() + wordArr[i].slice(1);
      }else{
        newStr += wordArr[i]
      }
    }
  }else{
    return newStr
  }
  return newStr;
}
```
3. ## Unique In Order exercise
```javascript
var uniqueInOrder=function(iterable){
   let strArr = Array.isArray(iterable) ? iterable : iterable.split('');
  let unique = strArr.filter((letter, i) => {
    return strArr[i] != strArr[i+1];
  })

  return unique;
}
```
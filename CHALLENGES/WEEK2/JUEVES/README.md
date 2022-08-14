1. ## Follow up with the HTML course you started on Tuesday
Finished
2. ## Remove All Exclamation Marks From The End Of Sentence exercise
```javascript
function remove (string) { 
  return string.replace(/!+$/, '');
}
```
3. ## Vowel Remover exercise
```javascript
function shortcut (string) {
 var respuesta =  string.replace(/[aeiou]/g, '');
  return respuesta ;
}
```
4. ## Rock Paper Scissors! exercise
```javascript
const rps = (p1, p2) => {
if (p1=== p2){
  return "Draw!"
  }
if (p1 === 'scissors'&& p2=== 'paper') {
  return "Player 1 won!"}
  
if(p1==="rock"&&p2==="scissors"){
  return "Player 1 won!"
}
if(p1 ==="paper"&&p2==="rock"){
  return "Player 1 won!"
}

if (p2 === 'scissors'&& p1=== 'paper') {
  return "Player 2 won!"}
  
if(p2==="rock"&&p1==="scissors"){
  return "Player 2 won!"
}
if(p2 ==="paper"&&p1==="rock"){
  return "Player 2 won!"
}

};
```
5. ## Persistent Bugger exercise
```javascript
function persistence(num) {
   //code me
  var numString = num.toString();
  var numDigitsCount = numString.length;
  var numMultCount = 0;
  
  while(numDigitsCount > 1){
    var numMultResult = 1;
   for(var i =0; i<= numString.length -1; i++){ //ultima posicion valida
     numMultResult = numMultResult * Number(numString[i]);
    }
  num = numMultResult;
  numMultCount = numMultCount + 1;
  numString = num.toString();
  numDigitsCount = numString.length;
}
  return numMultCount;

}
```
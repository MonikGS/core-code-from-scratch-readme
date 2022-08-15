
1. ## Simple Pig Latin exercise
```javascript
function pigIt(str){
  let array = str.split(" "); //separar palabras
  let newArr = [] //añadir array
  newStr = ""; // nueva palabra
  for (let i = 0; i < array.length; i++){
      newStr = array[i].slice(1) + array[i].charAt(0) + "ay"; //con cada palabra
      newArr.push(newStr); // agregar cambio
    } return newArr.join(" ")
}
```
2. ## Counting Duplicates exercise
```javascript

function duplicateCount(text) {
  let textArray = text.toLowerCase().split('').sort(); //orden, separacion y quitar mayusculas
  let i = 0,
    result = 0,
    lastIndexOfChar = 0; 
  while (textArray.length) {
    lastIndexOfChar = textArray.lastIndexOf(textArray[i]); //ver la posicion 
    if (lastIndexOfChar !== i) { 
      i = lastIndexOfChar;
      result++;
    }
    textArray = textArray.slice(++i);
    i = 0;
  }
  return result;
}
```
Other option
```javascript
function duplicationCount(text){
  return text.toLowerCase().split('').filter((val, i, arr) => {
    return arr.indexOf(val) !== i && arr.lastIndexOf(val) === i;
  }).length;
}
```
3. ## Decode The Morse Code exercise
```javascript
decodeMorse = function(morseCode){
  var words = (morseCode).split('  ');
  var letters = words.map((w) => w.split(' '));
  var decoded = [];

  for(var i = 0; i < letters.length; i++){
    decoded[i] = [];
    for(var x = 0; x < letters[i].length; x++){
        if(MORSE_CODE[letters[i][x]]){
            decoded[i].push( MORSE_CODE[letters[i][x]] );
        }
    }
  }

  return decoded.map(arr => arr.join('')).join(' ');
}
```
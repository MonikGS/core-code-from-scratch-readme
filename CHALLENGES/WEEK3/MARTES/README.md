
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
3. ## Decode The Morse Code exercise
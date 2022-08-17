1. ## Fold An Array exercise
```javascript
function foldArray(array, runs) {
    if (array.length == 1) return array;

    let newArray = [];
    let cantidadRepeticiones = parseInt(array.length / 2)
    console.log(cantidadRepeticiones)
    for (let i = 0; i < cantidadRepeticiones; i++) {
        newArray.push(array[i] + array[(array.length - 1 - i)])
    }

    if (array.length % 2 !== 0) newArray.push(array[cantidadRepeticiones]);

    if (runs > 1) {
        runs--
        return foldArray(newArray, runs)
    }

    return newArray;
}
```
2. ## Encrypt This! exercise
```javascript 
function encryptedWord(word) {
  if (word.length == 1) return word.charCodeAt();
  if (word.length == 2) return `${word.charCodeAt(0)}${word[1]}`;
  return `${word.charCodeAt(0)}${word[word.length - 1]}${word.slice(
    2,
    word.length - 1
  )}${word[1]}`;
}

var encryptThis = function (text) {
  return text.split(' ').map(encryptedWord).join(' ');
};
```
3. ## Complete your 1st Core Challenge. This is one of the requirements for the certification, where you'll boost your dev professional-brand.
I am Monica, an eletronic engineer student, I’ve been learning about programming languages, this is my first time using JavaScript, React & Node.js. I’m looking forward to  expand my knowledge and grow as a developer, along with my actual electronic career. 

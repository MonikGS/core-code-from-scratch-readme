1. ## Start this HTML course
Return to start of the repository

2. ## Multiply exercise
```javascript
function multiply(a, b){
return a * b; //siempre tener un return si se usa function
}
```

3. ## ASCII Total exercise
```javascript
function uniTotal (palabra) {
let conteo = palabra.length;
let suma = 0;
for(let i = 0; i < conteo; i++){
  suma = palabra.charCodeAt[i]+suma;
  }
  return suma;
}
```
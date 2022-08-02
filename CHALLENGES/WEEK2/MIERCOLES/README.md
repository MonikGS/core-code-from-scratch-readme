1. ##  Follow up with the HTML course you started on Tuesday
[HTML](SESION/README.md)

2. ## Char From ASCII Value exercise
```javascript
function getChar(c){
 return String.fromCharCode(c);// ...
}
```

3. ## Binary Addition exercise
```javascript
function addBinary(a,b) {
let suma = a+b;
return suma.toString(2);
}
```

4. ## Student's Final Grade exercise
```javascript
function finalGrade (exam, projects) {
    if (exam > 90 || projects > 10) {
        return 100// final grade
    } else if (exam > 75 && projects >= 5) {
        return 90
    } else if (exam > 50 && projects >= 2) {
        return 75
    }
    return 0;
}
```
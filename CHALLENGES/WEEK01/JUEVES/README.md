1. ### Print special numbers
- For
```javascript
for (let i = 0; i <= 100; i++) {
 if(i % 2 == 0) console.log(i);
}
```
- While
```javascript
let i= 0;
while (i <= 100) {
  i++;
 if(i % 2 == 0) console.log(i);
}
```
- do While
```javascript
let i = 0;
do {
  if(i % 2 == 0) console.log(i); 
  i ++;
}
while (i > 0 && i <= 100);
```

2. ### Bad Code
The error is missing a = to be a equality operator ( == ) checks whether its two operands are equal, returning a Boolean result. 

```javascript
var cond = false;

if ((cond == true)){
console.log('The cond variable is true');
}else {
  console.log('The cond variable is false');
}
```
3. ### Bad Code 2
The erros are the use of else if and connect the two conditional with and gate.
```javascript
var n = 100;

if (n == 100) {
  console.log('This is a special number!');
} else if (n < 1000 && n % 10 == 0 ) {
  console.log('This number is almost special');
} else {
   console.log('Just a regular number');
}
```
4. ### Follow Git Course
I'm already started 
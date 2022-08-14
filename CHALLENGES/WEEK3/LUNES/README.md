1. ## Who Likes It? exercise
```javascript
function likes(names) {
  if (names.length == 0){
    return 'no one likes this';
  } 
  if (names.length == 1){
    return names[0] + ' likes this';
    }
  if (names.length == 2) {
    return names[0] + ' and ' + names[1] + ' like this';
    }
  if (names.length == 3){
    return names[0] + ', ' + names[1] + ' and ' + names[2] + ' like this';
    }
  else{
  return ( names[0] +  ', ' + names[1] + ' and ' + (names.length - 2) + ' others like this');
    }
}
```
2. ## Bit Counting exercise
```javascript
var countBits = function(n) {
if (n>=0){
    // make an array with the bit result
   const base = (n).toString(2).split('');
   
   // make a sum with the array and make the index a Number
   const result = base.reduce((a, b) => a + Number(b), 0);
   
   return result; 
}
else{
var nn = n*-1;
     const base = (nn).toString(2).split('');
   
   // make a sum with the array and make the index a Number
   const result = base.reduce((a, b) => a + Number(b), 0);
   
   return result; 
}
};
```
3. ## Your Order, Please exercise
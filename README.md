# Intermediate Algorithm Scripting (FreeCodeCamp) Solutions

### sum all numbers in a range
```javascript
function sumAll(arr) {
   let start = (arr[0] > arr[1]) ? arr.shift() : arr.pop(), 
       end = arr.pop(),
       sum = 0;
    while(start >= end){
        sum += start;
        start--;
    }
    return sum;
}
```

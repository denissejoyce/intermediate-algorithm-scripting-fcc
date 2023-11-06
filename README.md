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

### diff two arrays
```javascript
function diffArray(arr1, arr2) {
  const newArr = [];
    for(item of arr1){
        if(arr2.indexOf(item) < 0){
            newArr.push(item);
        }
    }
    for(item of arr2){
        if(arr1.indexOf(item) < 0){
            newArr.push(item);
        }
    }
  return newArr;
}
```

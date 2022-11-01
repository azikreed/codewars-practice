1. **Removing Elements**

Take an array and remove every second element from the array. Always keep the first element and start removing with the next element.

## **Example:**

```js
["Keep", "Remove", "Keep", "Remove", "Keep", ...] --> ["Keep", "Keep", "Keep", ...]
```

None of the arrays will be empty, so you don't have to worry about that!

> **Solution**

```js
function removeEveryOther(arr) {
    let filtered = arr.filter((value, index) => {
        return index % 2 === 0;
    });
    return filtered
}
```

2. **Beginner - Lost Without a Map**

Given an array of integers, return a new array with each value doubled.

## **For example:**

```js
[1, 2, 3] --> [2, 4, 6]
```

> **Solution**

```js
function maps(x){
  let result = [];
  for(let i = 0; i < x.length; i++) {
    result.push(x[i]*2);
  }
  return result;
}
```
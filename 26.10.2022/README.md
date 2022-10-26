1. **Return Negative**

In this simple assignment you are given a number and have to make it negative. But maybe the number is already negative?

## **Examples**

```js
makeNegative(1);    // return -1
makeNegative(-5);   // return -5
makeNegative(0);    // return 0
makeNegative(0.12); // return -0.12
```

> **Solution**

```js
function makeNegative(num) {
  return num > 0 ? -num : num === 0 ? 0 : num;
}
```

2. **Find the Remainder**

Write a function that accepts two integers and returns the remainder of dividing the larger value by the smaller value.

Division by zero should return `NaN`.

## **Examples:**

```js
n = 17
m = 5
result = 2 (remainder of `17 / 5`)

n = 13
m = 72
result = 7 (remainder of `72 / 13`)

n = 0
m = -1
result = 0 (remainder of `0 / -1`)

n = 0
m = 1
result - division by zero (refer to the specifications on how to handle this in your language)

```

> **Solution**

```js
function remainder(n, m){
  let max = Math.max(n, m);
  let min = Math.min(n, m);
  return max % min;
}
```
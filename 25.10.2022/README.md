1. **Count Odd Numbers below n**

Given a number `n`, return the number of positive odd numbers below `n`, EASY!

## **Examples (Input -> Output)**
```js
7  -> 3 (because odd numbers below 7 are [1, 3, 5])
15 -> 7 (because odd numbers below 15 are [1, 3, 5, 7, 9, 11, 13])
```

Expect large Inputs!

> **Solution**

```js
function oddCount(n){
  return Math.floor(n/2);
}
```

2. **The 'if' function**

Create a function called `_if` which takes 3 arguments: a boolean value `bool` and 2 functions (which do not take any parameters): `func1` and `func2`

When `bool` is truth-ish, `func1` should be called, otherwise call the `func2`.

## **Example:**

```js
_if(true, function(){console.log("True")}, function(){console.log("false")})
// Logs 'True' to the console.
```

> **Solution**

```js
function _if(bool, func1, func2) {
  bool ? func1() : func2()
}
```
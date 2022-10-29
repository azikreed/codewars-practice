1. **Gravity Flip**

If you've completed this kata already and want a bigger challenge, here's the 3D version

Bob is bored during his physics lessons so he's built himself a toy box to help pass the time. The box is special because it has the ability to change gravity.

There are some columns of toy cubes in the box arranged in a line. The `i`-th column contains `a_i` cubes. At first, the gravity in the box is pulling the cubes downwards. When Bob switches the gravity, it begins to pull all the cubes to a certain side of the box, `d`, which can be either `'L'` or `'R'` (left or right). Below is an example of what a box of cubes might look like before and after switching gravity.

```
+---+                                       +---+
|   |                                       |   |
+---+                                       +---+
+---++---+     +---+              +---++---++---+
|   ||   |     |   |   -->        |   ||   ||   |
+---++---+     +---+              +---++---++---+
+---++---++---++---+         +---++---++---++---+
|   ||   ||   ||   |         |   ||   ||   ||   |
+---++---++---++---+         +---++---++---++---+
```

Given the initial configuration of the cubes in the box, find out how many cubes are in each of the n columns after Bob switches the gravity.

## **Examples (input -> output:**

```js
* 'R', [3, 2, 1, 2]      ->  [1, 2, 2, 3]
* 'L', [1, 4, 5, 3, 5 ]  ->  [5, 5, 4, 3, 1]
```

> **Solution**

```js
const flip=(d, a)=>{
  let result = [];
  if(d === "R") {
    result = a.sort((a,b) => {
      return a - b;
    });
  } else if (d === "L") {
    result = a.sort((a,b) => {
      return a - b;
    }).reverse();
  }
  
  return result;
}
```

2. **String repeat**

Write a function that accepts an integer `n` and a string `s` as parameters, and returns a string of `s` repeated exactly `n` times.

## **Examples (input -> output)**

```js
6, "I"     -> "IIIIII"
5, "Hello" -> "HelloHelloHelloHelloHello"
```

> **Solution**

```js
function repeatStr (n, s) {
  let result = "";
  for(let i = 0; i < n; i++) {
    result += s;
  }
  return result;
}
```

3. **You only need one - Beginner**

You will be given an array `a` and a value `x`. All you need to do is check whether the provided array contains the value.

Array can contain numbers or strings. X can be either.

Return `true` if the array contains the value, `false` if not.

> **Solution**

```js
function check(a, x) {
  return a.includes(x);
}
```
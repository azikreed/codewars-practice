1. **Vowel Count**

Return the number (count) of vowels in the given string.

We will consider `a`, `e`, `i`, `o`, `u` as vowels for this Kata (but not `y`).

The input string will only consist of lower case letters and/or spaces.

> **Solution**

```js
function getCount(str) {
  let result = 0;
  for(let i = 0; i < str.length; i++) {
    switch(str[i]) {
        case "a":
        case "e":
        case "i":
        case "o":
        case "u":
          result += 1;
          break
    }
  }
  return result;
}
```

2. **My head is at the wrong end!**


You're at the zoo... all the meerkats look weird. Something has gone terribly wrong - someone has gone and switched their heads and tails around!

Save the animals by switching them back. You will be given an array which will have three values (tail, body, head). It is your job to re-arrange the array so that the animal is the right way round (head, body, tail).

Same goes for all the other arrays/lists that you will get in the tests: you have to change the element positions with the same exact logics

Simples!

> **Solutions**

```js
function fixTheMeerkat(arr) {
  let result = [];
  for(let i = arr.length - 1; i >= 0; i--) {
    result.push(arr[i]);
  }
  return result;
}
```

```js
function fixTheMeerkat(arr) {
  return arr.reverse();
}
```
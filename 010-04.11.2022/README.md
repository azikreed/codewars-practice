1. **shorter concat [reverse longer]**

Given 2 strings, `a` and `b`, return a string of the form: `shorter+reverse(longer)+shorter.`

In other words, the shortest string has to be put as prefix and as suffix of the reverse of the longest.

Strings `a` and `b` may be empty, but not null (In C# strings may also be null. Treat them as if they are empty.).
If `a` and `b` have the same length treat `a` as the longer producing `b+reverse(a)+b`

> **Solution**

```js
function shorter_reverse_longer(a,b){
  if(a.length >= b.length) {
    return b + a.split("").reverse().join("") + b;
  } else {
    return a + b.split("").reverse().join("") + a;
  }
}
```

2. **Convert a String to a Number!**

Note: This kata is inspired by Convert a Number to a String!. Try that one too.

## **Description**

We need a function that can transform a string into a number. What ways of achieving this do you know?

Note: Don't worry, all inputs will be strings, and every string is a perfectly valid representation of an integral number.

## **Examples**

```js
"1234" --> 1234
"605"  --> 605
"1405" --> 1405
"-7" --> -7
```

> **Solution**

```js
const stringToNumber = function(str){
  return +str;
}
```


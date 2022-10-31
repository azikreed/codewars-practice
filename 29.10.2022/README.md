1. **Vowel remover**

Create a function called `shortcut` to remove the lowercase vowels (`a`, `e`, `i`, `o`, `u` ) in a given string.

## **Examples**

```js
"hello"     -->  "hll"
"codewars"  -->  "cdwrs"
"goodbye"   -->  "gdby"
"HELLO"     -->  "HELLO"
```

> **Solution**

```js
function shortcut (string) {
  return string.replace(/[aeiou]/gi, '');
}
```

2. **5 without numbers !!**

Write a function that always returns 5

Sounds easy right? Just bear in mind that you can't use any of the following characters: 0123456789*+-/

Good luck :)

> **Solution**

```js
function unusualFive() {
let five = 'Five!';
return five.length;
}
```
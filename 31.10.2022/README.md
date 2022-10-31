1. **How good are you really?**

There was a test in your class and you passed it. Congratulations!
But you're an ambitious person. You want to know if you're better than the average student in your class.

You receive an array with your peers' test scores. Now calculate the average and compare your score!

Return `True` if you're better, else `False`!

### **Note:**
Your points are not included in the array of your class's points. For calculating the average point you may add your point to the given array!

> **Solution**

```js
function betterThanAverage(classPoints, yourPoints) {
  return yourPoints > classPoints.reduce((a, b) => a + b) / classPoints.length;
}
```

2. **Vowel remover**

Create a function called `shortcut` to remove the **lowercase** vowels (`a`, `e`, `i`, `o`, `u` ) in a given string.

## **Examples**

```js
"hello"     -->  "hll"
"codewars"  -->  "cdwrs"
"goodbye"   -->  "gdby"
"HELLO"     -->  "HELLO"
```

- don't worry about uppercase vowels
- `y` is not considered a vowel for this kata

> **Solution**

```js
function shortcut (string) {
  return string.replace(/[aeiou]/gi, '');
}
```
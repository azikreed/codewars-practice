1. **A wolf in sheep's clothing**

Wolves have been reintroduced to Great Britain. You are a sheep farmer, and are now plagued by wolves which pretend to be sheep. Fortunately, you are good at spotting them.

Warn the sheep in front of the wolf that it is about to be eaten. Remember that you are standing at the front of the queue which is at the end of the array:

```js
[sheep, sheep, sheep, sheep, sheep, wolf, sheep, sheep]      (YOU ARE HERE AT THE FRONT OF THE QUEUE)
   7      6      5      4      3            2      1
```

If the wolf is the closest animal to you, return `"Pls go away and stop eating my sheep"`. Otherwise, return `"Oi! Sheep number N! You are about to be eaten by a wolf!"` where `N` is the sheep's position in the queue.

**Note**: there will always be exactly one wolf in the array.

## **Examples**

Input: `["sheep", "sheep", "sheep", "wolf", "sheep"]`
Output: `"Oi! Sheep number 1! You are about to be eaten by a wolf!"`

Input: `["sheep", "sheep", "wolf"]`
Output: `"Pls go away and stop eating my sheep"`

> **Solution**

```js
function warnTheSheep(queue) {
  let wolfIndex = queue.indexOf("wolf");
  let lengthOfArray = queue.length;
  if( wolfIndex === (lengthOfArray - 1)) {
    return "Pls go away and stop eating my sheep";
  } else {
    return `Oi! Sheep number ${lengthOfArray - (wolfIndex + 1)}! You are about to be eaten by a wolf!`
  }
}
```

1. **Twice as old**

   1. Your function takes two arguments:

   2. current father's age (years)

current age of his son (years)
Сalculate how many years ago the father was twice as old as his son (or in how many years he will be twice as old). The answer is always greater or equal to 0, no matter if it was in the past or it is in the future.

> **Solution**

```js
function twiceAsOld(dadYearsOld, sonYearsOld) {
  if(sonYearsOld * 2 > dadYearsOld) {
    return sonYearsOld * 2 - dadYearsOld;
  } else {
    return dadYearsOld - sonYearsOld * 2;
  }
}
```


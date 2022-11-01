1. **Pillars**

There are pillars near the road. The distance between the pillars is the same and the width of the pillars is the same. Your function accepts three arguments:

1. number of pillars (≥ 1);
2. distance between pillars (10 - 30 meters);
3. width of the pillar (10 - 50 centimeters).

Calculate the distance between the first and the last pillar in centimeters (without the width of the first and last pillar).

> **Solution**

```js
function pillars(numPill, dist, width) {
  return numPill !== 1 ? +(((numPill-2) * width) + (numPill-1)*dist*100) : 0
}
```

2. **No Loops 2 - You only need one**

You will be given an array `a` and a value `x`. All you need to do is check whether the provided array contains the value, without using a loop.

Array can contain numbers or strings. `x` can be either. Return `true` if the array contains the value, `false` if not. With strings you will need to account for case.

Looking for more, loop-restrained fun? Check out the other kata in the series:

> **Solution**

```js
function check(a,x){
  return a.includes(x);
};
```
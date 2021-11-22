## There are 7 basic types in JavaScript.

- number for numbers of any kind: integer or floating-point.
- string for strings. A string may have one or more characters, there’s no separate single-character
  type.
- boolean for true/false.
- null for unknown values – a standalone type that has a single value null.
- undefined for unassigned values – a standalone type that has a single value undefined.
- object for more complex data structures.
- symbol for unique identifiers.

The typeof operator allows us to see which type is stored in the variable.

- Two forms: typeof x or typeof(x).
- Returns a string with the name of the type, like "string".
- For null returns "object" – that’s an error in the language, it’s not an object in fact.

In the next chapters we’ll concentrate on primitive values and once we’re familiar with them, then
we’ll move on to objects.

## Difference between POST and GET, what does UPDATE and DELETE do

## Ajax vs Promise vs async & await
https://medium.com/front-end-weekly/ajax-async-callback-promise-e98f8074ebd7

## Event object, 3 ways add browser event, e.g. click. Check out summary.
https://javascript.info/introduction-browser-events#event-object

## Destructuring
**Array destructuring**

```js
// Variable assignment.
const foo = ["one", "two", "three"];

const [one, two, three] = foo;
console.log(one); // "one"
console.log(two); // "two"
console.log(three); // "three"
```

```js
// Swapping variables
let a = 1;
let b = 3;

[a, b] = [b, a];
console.log(a); // 3
console.log(b); // 1
```

**Object destructuring**

```js
// Variable assignment.
const o = { p: 42, q: true };
const { p, q } = o;

console.log(p); // 42
console.log(q); // true
```

## IIFE: http://lucybain.com/blog/2014/immediately-invoked-function-expression/

```js
(function foo(){ })()
```


##`forEach`

- Iterates through the elements in an array.
- Executes a callback for each element.
- Does not return a value.

```js
const a = [1, 2, 3];
const doubled = a.forEach((num, index) => {
  // Do something with num and/or index.
});

// doubled = undefined
```

##`map`

- Iterates through the elements in an array.
- "Maps" each element to a new element by calling the function on each element, creating a new array
  as a result.

```js
const a = [1, 2, 3];
const doubled = a.map((num) => {
  return num * 2;
});

// doubled = [2, 4, 6]
```

The main difference between `.forEach` and `.map()` is that `.map()` returns a new array. If you
need the result, but do not wish to mutate the original array, `.map()` is the clear choice. If you
simply need to iterate over an array, `forEach` is a fine choice.

## Numeric sort

```js
var points = [40, 100, 1, 5, 25, 10];
points.sort(function (a, b) {
  return a - b;
});
```

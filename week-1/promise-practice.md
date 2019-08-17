complete these exercises from javascript.info and paste your solutions in to this file:
* [promise basics](https://javascript.info/promise-basics#tasks)
* [promise chaining](https://javascript.info/promise-chaining#tasks) 
* [promise api](https://javascript.info/promise-api)

and here's another [helpful resources](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Using_promises)


## Promise Basics
#### Re-resolve a promise
What’s the output of the code below?
```js
let promise = new Promise(function(resolve, reject) {
  resolve(1);

  setTimeout(() => resolve(2), 1000);
});

promise.then(alert);
```
It is 1. there should be one argument in resolve/reject so just the first one is taken into account.

#### Delay with a promise

The function delay(ms) should return a promise. That promise should resolve after ms milliseconds, so that we can add .then to it, like this:
```js
function delay(ms) {
  return new Promise(resolve => setTimeout(resolve, ms));
}

delay(3000).then(() => alert('runs after 3 seconds'));

```
#### Animated circle with promise
```js


```

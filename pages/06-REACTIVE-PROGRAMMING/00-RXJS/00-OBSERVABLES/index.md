### Observables

Based on the [official RXJS documentation](https://rxjs.dev/guide/observable):



|       | SINGLE   | MULTIPLE
|-------|----------|-------
| Pull	| Function |	Iterator
| Push	| Promise  |	Observable

> Observables are lazy Push collections of multiple values.

Main concepts here are:

````md magic-move
```ts
// Creation
const observable = new Observable(/* */);
```
```ts
const observable = new Observable(function subscribe(subscriber) {
  const id = setInterval(() => {
    subscriber.next(Math.random()); // Executing
  }, 1000);
});
```
```ts
// Subscribing
const subscription = observable.subscribe((x) => console.log(x));
```

```ts
const subscription = observable.subscribe((x) => console.log(x));
// Unsubscribing
subscription.unsuscribe();
```
````

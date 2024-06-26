## RXJS and Observables

Reactive programming is an async programming paradigm centered on data streams and propagation of change.


```ts
import { . . . } from 'rxjs';
```

Most common operators are `map`, `take`, `takeUntil`, `of` and `filter`.

For example, let's say you have an observable, then you can pipe functions to combine, transform or filter the data as:

```ts
anObservale.pipe(
  filter(res => /* */),
  map(res => /* */),
);
```

You may argue this methods can also be executed on JavaScript, the focus is to use it thinking on the Observer design pattern, so when data arrives, these methods are called.

It is also a way to remove the `async` / `await` from your code and improve readability on async streams of data.

---
src: ./00-OBSERVABLES/index.md
---

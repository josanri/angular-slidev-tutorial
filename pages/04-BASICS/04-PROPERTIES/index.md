# Properties

To share data between between components parent and children there are two main properties:

##### `Input`

```ts
@Input() clicks: int;
```
Input decorator marks a property as a value that can be added to that component.

<hr class="mt-2 mb-2"/>


##### `Output`

```ts
@Output() name: EventEmitter<string>;
```
Output decorator marks a property as a value that can be emitted to the parent component.


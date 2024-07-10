# Properties

To share data between parent and children components (data binding) there are two main properties and decorators:

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


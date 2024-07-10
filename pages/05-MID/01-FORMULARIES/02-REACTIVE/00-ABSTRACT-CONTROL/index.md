### Reactive formularies
Everything comes from an abstract conrtol

```ts
export class MyNameFormControlComponent {
  name = new FormControl('');
}
```

```html
<input id="name" type="text" [formControl]="name">
```


```ts
export class MyFormComponent {
  myForm = new FormGroup({
    title: new FormControl(''),
    name: new FormControl(''),
  });
}

*You must import the `ReactiveFormsModule` at your module.*

### Reactive formularies
Everything comes froma n abstract conrtol

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

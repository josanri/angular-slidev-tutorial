## One-way data binding 📥 / 📤

### Input \[📥\]

From parent property to child component:

```html
<my-component [name]="name"></my-component>
```

<hr>

### Output (📤)

From child property to parent component:

```html
<my-component (newNameEvent)="handleEvent($event)"></my-component>
```

<hr>



## Data binding
Angular data binding con go on input, output or both:

### Input [📥]

From parent to child component:

```html
<my-component [name]="name"></my-component>
```

<hr>

### Output (📤)

From child to parent component:

```html
<my-component (newNameEvent)="handleEvent($event)"></my-component>
```

<hr>

### Two-Way data binding [(🍌)]
Also called banana in a box due to its shape, it goes from parent to child and child to parent component:

```html
<my-component [(name)]="name"></my-component>
```

<style>
    h4 {
        font-weight: bold;
        text-decoration: underline;
    } 
</style>
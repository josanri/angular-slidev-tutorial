## Two-Way data binding \[(🍌)\]
Also called banana in a box due to its shape, it goes from parent property to child and child property to parent component:

```html
<my-component [(name)]="name"></my-component>
```

## Data binding considerations

When using data binding we will be writing ``Typescript`` inside the quotes. There we will have access to properties from the component. If we want to use a constant we will have to write it as on Typescript In other words.

````md magic-move

```html
<!-- This is wrong as This is my name is not a variable from the component -->
<my-component [name]="This is my name"></my-component>
```

```html
<!-- Quotes added -->
<!-- This is okay as 'This is my name' is a constant -->
<my-component [name]="'This is my name'"></my-component>
```

````


<style>
    h4 {
        font-weight: bold;
        text-decoration: underline;
    } 
</style>
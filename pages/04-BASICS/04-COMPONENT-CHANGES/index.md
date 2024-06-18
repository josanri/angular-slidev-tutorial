#### `ngOnChanges`, interface `OnChanges`
```ts
ngOnChanges(){
  // Change your component
}
```

#### Javascript `setters`
It's better for code manteinance to use setters instead of multiple `ngOnChanges` conditions. Like this:

```ts
 @Input()
 set example(msg) {
    if (msg === 0)
      this.example = 1;
    else
      this.example = msg;
  }
```

, with this you can specify input control in a better way.


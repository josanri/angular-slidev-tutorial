## Styles

### ngClass
Adds the `css` class conditionally:
```html
<div [ngClass]="{'pt-2': true, 'container': true, 'green': false}">
  <!-- More content-->
</div>
```
This can be useful when using class properties to activate or deactivate classes programatically.

### ngStyle
Same, but with `css` styles.
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

Same, but with `css` styles:

```html
<div [ngStyle]="{'padding-top': '2px', 'display': 'flex', 'color': 'green'}">
  <!-- More content-->
</div>
```

> There is no need to change property names, you can use the same one as in css, but if you want to include the unit you can specify it as a suffix. For example `{'padding-top.px': '2', . . .}`, where unit can be `px` (pixels), `em` (relative to parent font size), `rem` (relative to root font size) or  `%` (percentage).
### Using function at templates expressions

Angular change detection is very smart, but does not know the future. Therefore, when a function is used inside a template expression, every change at the component will make the component call this component.

```html
<component *ngIf="isConditionTrue(name)">
</component>
```

Changing the detection method to `OnPush` may not be enough, so avoid doing so. Here are some alternatives:

+ **Pipes**: Instead of using a function, a pipe detects changes better than a function. It is a possibility though pipes are used for data transformation instead of conditions.

```html
<component *ngIf="name | isConditionPipe">
</component>
```

+ Using **properties** (not computed properties): conditions based on attributes or properties.

```html
<component *ngIf="name.length > 0">
</component>
```
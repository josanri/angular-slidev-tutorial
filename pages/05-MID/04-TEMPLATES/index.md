## Templates

### ng-container

The `<ng-container>` tag is used on components to specify where data could be interpolated from parent components as `{{ object }}`
```html
<ng-container></ng-container>
```

### ng-template

Avoid using a `<div>`, instead is replaced by inner content (similar to `<>` or `React.Fragment` at React).

````md magic-move

```html
<ng-template>
    <!-- Content --->
</ng-template>
```

```html
<div *ngIf="name else referenceToThisComponent">
    <!-- Can be used with directives as *ngIf to show conditionally a part of the page --->
</div>


<ng-template #referenceToThisComponent>
    <!-- Content --->
</ng-template>
```
````


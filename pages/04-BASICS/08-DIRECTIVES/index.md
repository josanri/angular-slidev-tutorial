## Directives
### ngIf

Sets a condition for the node to be rendered:

```html
  <p *ngIf="age>=18">You are an adult.</p>
```

Even set at the same part which will be the alternative text:

```html
  <p *ngIf="age>=18; else underBlock">You are an adult.</p>
  <ng-content #underBlock>You are under 18.</p>
```

### ngFor
Renders as many elements as the array contians:

```html
<ul *ngFor="let name of names">
  <li>{{ name }}</li>
</ul>
```


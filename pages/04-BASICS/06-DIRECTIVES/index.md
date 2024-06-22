## Directives
### ngIf
Sets a condition for the node to be rendered:
```html
  <p *ngIf="age>=18">You are an adult.</p>
```

### ngFor
Renders as many elements as the array contians:

```html
<ul *ngFor="let name of names">
  <li>{{ name }}</li>
</ul>
```


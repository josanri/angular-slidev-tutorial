## Pipes
Angular uses `pipes` to transform data before displaying it to the HTML.
```html
<span>{{ variable | pipe }}</span>
```

, where `pipe` can be:

- `date`
- `uppercase`
- `lowercase`
- `currency`
- `async`, to consume an observable
- . . .

For example:
```html
<span>{{ name | uppercase }}</span>
```

## Interpolation `{{ }}`

You can display values from component properties with curly brackets `{{ variable }}`

```html
<span>My name is: {{ name }}</span>
```

This can also be used inside quoted attributes:

```html
<a href="{{ imageUrl }}">Click here.</a>
```

The view will be updated if the property is changed.
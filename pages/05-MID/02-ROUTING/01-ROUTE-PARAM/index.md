###  Router Param

If you want to use router link here, you can add the segments of the URL as an array:

```html
<a [routerLink]="['/item', 1]">Item 1</a>
```

When you use a route like `item/:id` you want to use that information at the componnet, you use the `ActivatedRoute` on dependency injection:

````md magic-move
```ts
import { Router, ActivatedRoute, ParamMap } from '@angular/router';

@Component({
  standalone: true,
  selector: 'todo-list-item',
  templateUrl: './todo-list-item.component.html',
  styleUrl: './todo-list-item.component.css',
})
export class TodoListItem {
    constructor(
        private route: ActivatedRoute,
    ) {}
}
```
```ts
import { Router, ActivatedRoute, ParamMap } from '@angular/router';

@Component({
    // . . . 
})
export class TodoListItem {
    constructor(
        private route: ActivatedRoute,
    ) {}

    ngOnInit() {
        this.id = this.route.snapshot.paramMap.get('id'); // Get from path
    }
}
```

```
```ts
import { Router, ActivatedRoute, ParamMap } from '@angular/router';

@Component({
    // . . . 
})
export class TodoListItem {
    constructor(
        private route: ActivatedRoute,
    ) {}

    ngOnInit() {
        this.route.queryParams.subscribe(params => {
            this.name = params['name']; // Get from query parameters (?name=myName&...)
        });
    }
}
```
````

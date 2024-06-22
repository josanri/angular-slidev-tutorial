### Example

````md magic-move
```ts
import { Component } from "@angular/core";

@Component({
  standalone: true,
  selector: 'todo-list-item',
  templateUrl: './todo-list-item.component.html',
  styleUrl: './todo-list-item.component.css',
})
export class TodoListItem {
  /* Component behavior is defined in here */
}
```

```ts
import { Component, Input, Output, EventEmitter } from "@angular/core";

@Component({
  // . . .
})
export class TodoListItem {
  @Input() name: string;
  @Output() itemEvent = new EventEmitter<string>();
}
```

```ts
import { Component, Input, Output, EventEmitter } from "@angular/core";

@Component({
  // . . .
})
export class TodoListItem implements onInit {
  @Input() name: string;
  @Output() itemEvent = new EventEmitter<string>();

  constructor(){
    // Initialize value on constructor is not recommended
    // Leave constructor for dependency injection
    // this.name = "Default name";
  }
  
}
```

```ts
import { Component, Input, Output, EventEmitter } from "@angular/core";

@Component({
  // . . .
})
export class TodoListItem implements onInit {
  @Input() name: string;
  @Output() itemEvent = new EventEmitter<string>();

  constructor() { }
  
  ngInit(){
    this.name = "Default name"; // You can either initialize value on ngInit 
  }
  
}
```

```ts
import { Component, Input, Output, EventEmitter } from "@angular/core";

@Component({
  // . . .
})
export class TodoListItem implements onInit {
  @Input() name: string = "Default name"; // Or initialize at definition
  @Output() itemEvent = new EventEmitter<string>();

  constructor() { }

  ngInit(){
    // Logic on init
  }
}
```

```ts
import { Component, Input, Output, EventEmitter } from "@angular/core";

@Component({
  // . . .
})
export class TodoListItem implements onInit, onDestroy {
  @Input() name: string = "Default name";
  @Output() itemEvent = new EventEmitter<string>();

  constructor() { }

  ngInit(){
    // Logic on init
  }
  
  ngDestroy(){
    // Logic on destroy
  }
}
```

````
## Components

Defines the component structure, properties and style.

```ts {*|3,8|4|5|6|7} 
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

<ul>
<li v-click="2"> The <code>standalone</code> components do <strong>not need</strong> a module to be created.</li>
<li v-click="3"> The <code>selector</code> is the name other components will use to create the component, as a XHTML tag.</li> 
<li v-click="4"> The <code>template URL</code> has the "HTML" for the component. This is not HTML as it can be enriched with Angular sintaxis.</li> 
<li v-click="5"> The <code>style</code> URL has the <kbd>css</kbd>, <kbd>sass</kbd> or <kbd>scss</kbd> styles for the components. These styles are encapsulated for the component. If you want to  have the global styles, you will have to store them in a <code>global.css</code> file.</li>
</ul>


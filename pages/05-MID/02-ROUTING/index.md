## Routing

To start routing

````md magic-move
```ts
import { NgModule } from '@angular/core';
import { RouterModule, Routes } from '@angular/router';

const routes: Routes = [
  { path: 'to-do', component: TodoListComponent }
];

@NgModule({
  imports: [RouterModule.forRoot(routes)],
  exports: [RouterModule]
})
export class AppRoutingModule { }
```


```ts
import { NgModule } from '@angular/core';
import { RouterModule, Routes } from '@angular/router';

const routes: Routes = [
  { path: '', redirectTo: '/to-do', pathMatch: 'full' },
  { path: 'to-do', component: TodoListComponent },
  { path: 'item/:id', component: ItemComponent },
  { path: '**', component: 'PageNotFoundComponent' }
];

@NgModule({
  imports: [RouterModule.forRoot(routes)],
  exports: [RouterModule]
})
export class AppRoutingModule { }
```
````

<ul>
    <li v-click="2"><code>pathMatch:'full'</code>, when the remaining, unmatched segments of the URL match is the prefix path. The while URL matches.</li>
    <li v-click="3"><code>pathMatch:'prefix'</code>,  when the remaining URL begins with the redirect route's prefix path. The first segment of the path.</li>
</ul>

---
src: ./00-ROUTER-LINK/index.md
---

---
src: ./01-ROUTE-PARAM/index.md
---

---
src: ./02-GUARDS/index.md
---

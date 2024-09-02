###  Router Link

Using `routerLink` instead of `<a>` (anchor HTML tag) allows Angular to serve the application as a SPA, without refreshing the entire page.

```html
<nav>
    <a routerLink="/">Home</a>
    <a routerLink="/to-do">ToDo</a>
</nav>
```

### Router Outlet

The `router-outlet` means **where a subcomponent** will be. The rest of the HTML will be shared from parent to child component.

```html
<div>
    <router-outlet></router-outlet>
</div>
```

> Avoid using `router-outlet` or you'll init the component twice (`ngInit` is called twice but is not destroyed).

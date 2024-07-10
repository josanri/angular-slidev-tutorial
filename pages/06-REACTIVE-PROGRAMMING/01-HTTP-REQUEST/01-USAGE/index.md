### HTTP Requests Usage

Inside a service or component we may found the following structure. A client provided as dependency injection and a method to send and process requests:

```ts
    constructor(private http:HttpClient) {}
    
    sendRequest(){
      this.http.get<Type[]>(url)
        .map(data => /* Do something*/);
    }
```

Or you can subscribe to the observable and process data as:
````md magic-move
```ts
this.http.get<Type[]>(url).subscribe(data => /* Do something*/);
```
```ts
this.http.get<Type[]>(url).subscribe(
  {
    next: data => /* Do something*/,
    error: /* Control error*/
  }
);
```
````
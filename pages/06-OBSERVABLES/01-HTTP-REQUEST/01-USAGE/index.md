Inside a component we may found the following structure. A client provided as dependency injection and a method to send and process requests:
```ts
    constructor(private http:HttpClient) {}
    
    sendRequest(){
      this.http.get<Type[]>(url)
            .map(data => /* Do something*/);
    }
```
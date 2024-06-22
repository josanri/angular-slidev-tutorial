### HTTP Requests Interface

HTTP Requests are the most common way to gather and send information. In Javascript, `fetch` and `XMLHttpRequest` APIs can be used for HTTP requests. Nevertheless, as Angular is oriented to observables more than asynchronous code, `HttpClient` is provided as a class to send requests.


```ts
export declare class HttpClient {
    private handler;
    // . . .
    request(method: string, url: string, options: {
        body?: any;
        headers?: HttpHeaders | {
            [header: string]: string | string[];
        };
        context?: HttpContext;
        observe?: 'body';
        params?: HttpParams;
        reportProgress?: boolean;
        responseType: 'arraybuffer';
        withCredentials?: boolean;
        // ...
    }): Observable<ArrayBuffer>;
    // request, get, post, put, patch, delete...
}
```

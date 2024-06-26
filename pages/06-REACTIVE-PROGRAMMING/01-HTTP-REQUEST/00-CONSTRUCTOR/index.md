### HTTP Requests Interface

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

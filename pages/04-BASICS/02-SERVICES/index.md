## Services

Defines the component structure, properties and style.

```ts {*|3,5|4|*} 
import { Injectable } from "@angular/core";

@Injectable({
  providedIn: 'root',
})
export class TodoListAPI {
    constructor() { }
    /* Service behavior is defined in here */
}
```

<ul>
<li
 v-click="2"> The <code>providedIn</code> is used to define which injectors provide the injectable class, it may be <code>root</code>, <code>platform</code> or <code>any</code>.</li> 
<li v-click="3"> Services are commonly used by dependency injection on components that make use of them like this:</li> 
</ul>

<pre v-click="3" class="shiki shiki-themes vitesse-dark vitesse-light slidev-code" style="--shiki-dark: #dbd7caee; --shiki-light: #393a34; --shiki-dark-bg: #121212; --shiki-light-bg: #ffffff;"><code class="language-ts"><span class="line"><span style="--shiki-dark: #80A665; --shiki-light: #59873A;">    constructor</span><span style="--shiki-dark: #666666; --shiki-light: #999999;">(</span><span style="--shiki-dark: #BD976A; --shiki-light: #B07D48;">private</span><span style="--shiki-dark: #BD976A; --shiki-light: #B07D48;"> todoListAPI</span><span style="--shiki-dark: #DBD7CAEE; --shiki-light: #393A34;">: </span><span style="--shiki-dark: #BD976A; --shiki-light: #B07D48;">TodoListAPI</span><span style="--shiki-dark: #666666; --shiki-light: #999999;">)</span><span style="--shiki-dark: #666666; --shiki-light: #999999;"> {}</span></span></code></pre>

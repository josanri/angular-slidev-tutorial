## Modules

```ts {4,16|5|8|12|15} 
import { NgModule } from "@angular/core";

// app.module.ts
@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    FormsModule,
    // . . .
  ],
  providers: [
    // . . .
  ],
  bootstrap: [AppComponent]
})
export class AppModule {
}
```

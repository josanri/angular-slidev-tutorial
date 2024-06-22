## Modules

Sets the injector and compiler by identifying components, services and dependencies.

```ts {*|4,16|6|9|13|16} 
import { NgModule } from "@angular/core";

// app.module.ts
@NgModule({
  declarations: [
    AppComponent,
    // Components
  ],
  imports: [
    FormsModule,
    // Modules
  ],
  providers: [
    // Services
  ],
  bootstrap: [AppComponent]
})
export class AppModule {
}
```

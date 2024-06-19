### Template Driven


```html{*|3|5|7|1,11}
<form (ngSubmit)="onSubmit(formRef)" #formRef="ngForm">
    <label . . .>
        <input ngModel . . . />
    <label . . .>
        <input id="inputName" [(ngModel)]="model.name" . . . />
    <label . . .>
        <input id="inputdate" [(ngModel)]="model.name" . . .  #inputDate="ngModel" />
    <!--
    ...
    --->
        <input type="submit" />
</form>
```

<ul>
<li v-click="1"> Make use of <code>ngModel</code> binding.</li>
<li v-click="2"> Use two way-data data binding</li> 
<li v-click="3"> Use <code>onSubmit</code> to check event on submitting the form</li> 
<li v-click="4"> Adding a reference to the input will be useful when checking some properties we will se on the following slides</li> 
</ul>

*You must import the `FormsModule` at your module.*
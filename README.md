# angular
Angular Playground

<h2>Command line</h2>
Angular has a command line tool allowing to create projects, adding components, serving the application and many more.
See ng --help for more info

<h2>Big Picture</h2>
Typescript, super-set of Javascript, is used.

- Components: UI-Code consisting of HTML-template and Code, like Lego-Block
- Service: Reusable Code
- Modules: Organize Code

<img src=angular-elements.png"/>

<h2>Components</h2>
Consist of imports
```javascript
import {Component} from '@angular/core'</code>
```

Decorators
```javascript
@Component({
 selector: 'app-customer',
 templateUrl: '../customers.component.html'
 }}

Class
export class CustomerComponent {
}
 ```

<h2>Module</h2>
Every app has a least a model, like a container for legos

<h2>Property and Event Binding</h2>
 ```javascript
<h1 [hidden]="!isVisible">{{title}}</h1>
<button (click)="changeVisibility()">
 ```
Interpolation, Property binding, Event binding, Directive

 ```{{}} ```: Interpolation
 ```[] ```: Property binding
 ```(): ``` Event binding
 ```<tr *ngFor="let cust of filteredCustomers" ```: Directive

<h2>Best practices</h2>
- Add lint
- Protractor.js -> E2E-Tests
- Karma -> Junit-Testing
- .editconfig

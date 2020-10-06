## AngularJs LinkedIn Assesment Questions Answers (Left)

Q1. What is the purpose of the ViewChild decorator in this component class?

    @Component({
    . . .
    template: '<p #bio></p>'
    })
    export class UserDetailsComponent {
    @ViewChild('bio') bio;
    }

    a) It provides access from within the component class to the ElementRef object for the <p> tag that has the bio template reference variable in the component's   template view.It provides access from within the component class to the null object for the null tag that has the null template reference variable in the component's template view.
    b) It indicates that the <p> tag be rendered as a child of the parent view that uses this component.It indicates that the null tag be rendered as a child of the parent view that uses this component.
    c) It makes the <p> tag in the template support content projection.It makes the null tag in the template support content projection.
    d) It makes the <p> tag visible in the final render. If the #bio was used in the template and the @ViewChild was not used in the class, then Angular would automatically hide the <p> tag that has #bio on it.

Q2. How can you use the HttpClient to send a POST request to an endpoint from within an addOrder function in this OrderService?

    export class OrderService {
    constructor(private httpClient: HttpClient) { }

        addOrder(order: Order) {
            // Missing line
        }
        }

    a) this.httpClient.url(this.orderUrl).post(order);null
    b) this.httpClient.send(this.orderUrl, order);null
    c) this.httpClient.post<Order>(this.orderUrl, order);null
    d) this.httpClient.post<Order>(this.orderUrl, order) .subscribe();

Q3. What is the RouterModule.forRoot method used for?What is the null method used for?

    a) registering any providers that you intend to use in routed componentsregistering any providers that you intend to use in routed components
    b) registering route definitions at the root application levelregistering route definitions at the root application level
    c) indicating that Angular should cheer on your routes to be successfulindicating that Angular should cheer on your routes to be successful
    d) declaring that you intend to use routing only at the root level

Q4. Which DOM elements will this component metadata selector match on?

    @Component({
    selector: 'app-user-card',
    . . .
    })

    a) any element with the attribute app-user-card, such as <div app-user-card></div>any element with the attribute null, such as null
    b) the first instance of <app-user-card></app-user-card>the first instance of null
    c) all instances of <app-user-card></app-user-card>all instances of null
    d) all instances of <user-card></user-card>

Q5. What is the correct template syntax for using the built-in ngFor structural directive to render out a list of productNames?What is the correct template syntax for using the built-in null structural directive to render out a list of null?

    a)  <ul>
        <li [ngFor]="let productName of productNames">
            {{ productName }}
        </li>
        </ul>

    b)  <ul>
        <li ngFor="let productName of productNames">
            {{ productName }}
        </li>
        </ul>

    c)  <ul>
        <li *ngFor="let productName of productNames">
            {{ productName }}
        </li>
        </ul>

    d)  <ul>
        <? for productName in productNames { ?>
        <li>{{ productName }}</li>
        <? } ?>
        </ul>

Q6. What are the two component decorator metadata properties used to set up CSS styles for a component?What are the two component decorator metadata properties used to set up CSS styles for a component?

    a) viewEncapsulation and viewEncapsulationFilesnull and null
    b) There is only one and it is the property named css.There is only one and it is the property named null.
    c) css and cssUrlnull and null
    d) styles and styleUrlsnull and null

Q7. With the following component class, what template syntax would you use in the template to display the value of the title class field?

    @Component({
    selector: 'app-title-card',
    template: ''
    })
    class TitleCardComponent {
    title = 'User Data';
    }

    a) {{ 'title' }}null
    b) {{ title }}null
    c) [title]null
    d) A class field cannot be displayed in a template via the template syntax.

Q8. What is the purpose of the valueChanges method on a FormControl?What is the purpose of the null method on a null?

    a) It is used to configure what values are allowed for the control.It is used to configure what values are allowed for the control.
    b) It is used to change the value of a control to a new value. You would call that method and pass in the new value for the form field. It even supports passing in an array of values that can be set over time.It is used to change the value of a control to a new value. You would call that method and pass in the new value for the form field. It even supports passing in an array of values that can be set over time.
    c) It returns a Boolean based on if the value of the control is different from the value with which it was initialized.It returns a Boolean based on if the value of the control is different from the value with which it was initialized.
    d) It is an observable that emits every time the value of the control changes, so you can react to new values and make logic decisions at that time.It is an null that emits every time the value of the control changes, so you can react to new values and make logic decisions at that time.

Q9. What directive is used to link an <a> tag to routing?

    a) routeTo
    b) routerLink <---Correct
    c) routePathn
    d) appLink

Q10. What is the Output decorator used for in this component class?

    @Component({
    selector: 'app-shopping-cart',
    . . .
    })
    export class ShoppingCartComponent {
    @Output() itemTotalChanged = new EventEmitter();
    . . .
    }

    a) It makes the itemTotalChanged class field public.It makes the null class field public.
    b) It provides a way to bind values to the itemTotalChanged class field, like so: <app-shopping-cart [itemTotalChanged]="newTotal"></app-shopping-cart>.It provides a way to bind values to the null class field, like so: null.
    c) It provides a way to bind events to the itemTotalChanged class field, like so: <app-shopping-cart (itemTotalChanged)="logNewTotal($event)"></app-shopping-cart>.It provides a way to bind events to the null class field, like so: null.
    d) It is simply a way to put a comment in front of a class field for documentation.

Q11. What is the difference between these two markup examples for conditionally handling display?

    <div \*ngIf="isVisible">Active</div>
    <div [hidden]="!isVisible">Active</div>

    a) The ngIf is shorthand for the other example. When Angular processes that directive, it writes a div element to the DOM with the hidden property.The null is shorthand for the other example. When Angular processes that directive, it writes a null element to the DOM with the null property.
    b) They are fundamentally the same.They are fundamentally the same.
    c) The ngIf directive does not render the div in the DOM if the expression is false. The hidden property usage hides the div content in the browser viewport, but the div is still in the in the DOM.The null directive does not render the null in the DOM if the expression is null. The null property usage hides the null content in the browser viewport, but the null is still in the in the DOM.
    d) The ngIf is valid, but the use of the hidden property is wrong and will throw an error.

Q12. How can you disable the submit button when the form has errors in this template-driven forms example?

    <form #userForm="ngForm">
    <input type="text" ngModel name="firstName" required>
    <input type="text" ngModel name="lastName" required>
    <button (click)="submit(userForm.value)">Save</button>
    </form>

    a) <button (click)="submit(userForm.value)"
            disable="userForm.invalid">
            Save</button>

    b) <button (click)="submit(userForm.value)"
            [disabled]="userForm.invalid">
            Save</button>

    c) <button (click)="submit(userForm.value)"
            [ngForm.disabled]="userForm.valid">
            Save</button>

    d) <button (click)="submit(userForm.value)"
            *ngIf="userForm.valid">
            Save</button>

#### Q13. Pick the matching code for the custom provider registration that the @Inject() decorator is looking for:
```js
 constructor(@Inject('Logger') private logger) {}
```
   
- [ ] `providers: [ Logger ]`
   
- [ ] `@Injectable({ providedIn: 'root' })`
    
- [ ] `providers: [{ provide: 'Logger' }]` 

- [x] `providers: [{ provide: 'Logger', useClass: Logger }]` 


#### Q14. With the following TestBed setup, what can be used to access the rendered DOM for the UserCardComponent ?
```js
 TestBed.configureTestingModule({ 
   declarations: [ UserCardComponent ]
 });
 fixture = TestBed.createComponent(UserCardComponent);
```
   
- [ ] `fixture.getComponentHtml()`
   
- [ ] `fixture.nativeElement`
    
- [ ] `fixture.componentInstance.template` 

- [ ] `fixture.componentTemplate` 



#### Q15. For the following template-driven forms example, what argument can be passed to the submit() method in the click event to submit the data for the form ?

```css
<form #form="ngForm">
    <input type="text" ngModel name="firstName">
    <input type="text" ngModel name="lastName">
    <button (click)="submit()">Save</button>
</form>
```

- [ ]  `submit(form.value)`
  
- [ ]  `submit($event)`
  
- [ ]  `submit(firstName, lastName)`
  
- [ ]  `submit(ngForm.value)`

#### Q16. Based on the following usage of the async pipe, and assuming the users class field is an Observable, how many subcriptions to the users Observable are being made ?

```css
<h2>Names</h2>
<div *ngFor="let user of users | async">{{ user.name }}</div>
<h2>Ages</h2>
<div *ngFor="let user of users | async">{{ user.age }}</div>
<h2>Genders</h2>
<div *ngFor="let user of users | async">{{ user.gender }}</div>

```

- [ ]  `None. The async pipe does not subscribe automatically`
  
- [ ]  `One. the async pipe caches Observables by type internally`
  
- [ ]  `Three. There is one for each async pipe`
  
- [x]  `None. The template syntax is not correct`


#### Q17. What other template syntax (replacing the ngClass directive) can be used to add or remove the CSS class names in this markup ?

```css
<span
     [ngClass]="{ 'active': isActive, 'can-toggle': canToggle }">
  Employed
</span>

```

- [ ]  `<span
     [styles.class.active]="isActive"
     [styles.class.can-toggle]="canToggle">
  Employed
</span>`
  
- [ ]  `<span
     [class.active]="isActive"
     [class.can-toggle]="canToggle">
  Employed
</span>`
  
- [ ]  `<span
      class="{{ isActive ? 'is-active' : '' }}"
      class="{{ canToggle ? 'can-toggle' : '' }}">
  Employed
</span>`
  
- [ ]  `<span
     [css.class.active]="isActive"
     [css.class.can-toggle]="canToggle">
  Employed
</span>`


#### Q18. Given these two components, what will get rendered to the DOM based on the markup usage ?

```js
@Component({
   selector: 'app-card',
   template: '<h1>Data Card</h1><ng-content></ng-content>'
 })
 export class CardComponent { }
 
 @Component({
    selector: 'app-bio',
    template: '<ng-content></ng-content>'
  })
  export class BioComponent { }
  
  // markup usage
  <app-card><app-bio>Been around for four years.</app-bio></app-card>

```

- [ ] `<h1>Data Card</h1> <app-bio> Been around for four years. <app-bio>`
- [ ] `<app-card>
        <h1>Data Card</h1>
        <ng-content></ng-content>
        <app-bio>
         Been around for four years.
         <ng-content></ng-content>
        </app-bio>
       </app-card>`
- [ ] `<app-card>
        <h1>Data Card</h1>
       </app-card>`
- [ ] `<app-card>
        <h1>Data Card</h1>
        <app-bio>
         Been around for four years.
        </app-bio>
       </app-card>`
       

#### Q19. Given the app-title-card component in the code below, what DOM will the app-user-card component render ?

```js
@Component({
   selector: 'app-user-card',
   template: '<app-title-card></app-title-card><p>Jenny Smith</p>'
 })
 
 @Component({
    selector: 'app-title-card',
    template: '<h1>User Data</h1>'
  })
  
  // usage of user card component in parent component html
  <app-user-card></app-user-card>

```

- [ ] `<h1>User Data</h1><p>Jenny Smith</p>`
- [ ] `<app-user-card>
        <app-title-card>
         <h1>User Data</h1>
        </app-title-card>
        <p>Jenny Smith</p>
       </app-user-card>`
- [ ] `<div app-user-card>
        <h1 app-title-card>User Data</h1>
        <p>Jenny Smith</p>
       </div>`
- [ ] `<app-user-card>
        <app-title-card></app-title-card>
       </app-user-card>`
       

#### Q20. What are the Hostlistener decorators and the HostBinding decorator doing in this directive ?

```js
@Directive({
   selector: '[appCallout]'
 })
 export class CalloutDirective {
   @HostBinding('style.font-weight') fontWeight = 'normal';
   @HostListener('mouseenter') onMouseEnter() { this.fontWeight = 'bold' }
   @HostListener('mouseleave') onMouseLeave() { this.fontWeight = 'normal' }
 
 }
```

- [ ] `They are setting the CalloutDirective.fontWeight field based on whether or not the mouse is over the DOM element. The HostListener then sets the font-weight CSS property to the fontWeight value`
- [ ] `If the DOM element that this directive is placed on has the CSS property font-weight set on it, the mouseenter and mouseleave events will get raised.`
- [ ] `They are setting up the directive to check the DOM element that it is on. If it has event bindings added for mouse enter and leave, it will use this code. Otherwise nothing will happen`
- [ ] `This is an incorrect use of HostListener and HostBinding. the HostListener and HostBinding decorators do not do anything on directives; they work only when used on components`

#### Q21. Descripe the usage of this code:

```js
export interface AppSettings {
   title: string;
   version: number
}

export const APP_SETTINGS = new InjectionToken<AppSettings>('app.settings');
```

- [ ] `They InjectionToken is adding an instance of the AppSettings to the root provider via the InjectionToken constructor call, making it automatically available to all NgModules, services, and components throughout the Angular application without the need to inject it anywhere`
- [ ] `The InjectionToken is used to create a dynamic decorator for the AppSettings that can be used on constructor parameters via an @AppSettings decorator`
- [ ] `This code has an error since you cannot use a TypeScript interface for the generic type on the InjectionToken`
- [ ] `The InjectionToken is used to create a provider token for a non-class dependency. An object literal can be provided as a value for the APP_SETTINGS dependency provider type that can then be injected into components, service etc.`


#### Q22. Assuming the username FormControl has been configured with a minlength validator, how can you set up an error display in the following reactive forms markup for the username field ?

```js
<form [formGroup]="form">
  <input type="text" formControlName="username>
  . . .
<form>

```

- [ ] `
 <span *ngif="form.get('username').getError('minLength') as minLengthError">
   Username must be at least {{ minLengthError.requiredLength }} characters.
 </span>`
- [ ] `<input type="text" formControlName="username" [showMinLength]="true">`
- [ ] `
<input type="text" formControlName="username" #userName="ngModel">
<span *ngif="userName.errors.minlength">
   Username must be at least {{ userName.errors.minlength.requiredLength }} characters.
 </span>`
- [ ] `
<span *ngif="username.minLength.invalid">
   Username length is not valid.
 </span>`
 
 
 #### Q23. When a service is provided for root and is also added to the provider's configuration for a lazy-loaded module, what instance of that service does the injector provide to constructors in the lazy-loaded module ?

- [ ] `A single instance of that service is always instantiated at root and is the only one ever used, including within lazy modules.`
- [ ] `A new instance of that service is created when the module is lazy loaded.`
- [ ] `If an instance of the service has not been created at the root level yet, it will create one there and then use it.`
- [ ] `Providing a service of the same type at a lazy-loaded module level is not allowed`

#### Q24. Which template interpolation expression is valid ?

```js
{{ 'Today is the day' }}

{{ 10 + 5 }}

{{ myCount++ }}

```

- [ ] `both of these answers`
- [ ] `only {{ 'Today is the day' }}`
- [ ] `neither of these answers`
- [ ] `both {{ 'Today is the day' }} and {{ 10 + 5 }}`

#### Q25. What is the difference between the paramMap and the queryParamMap on the ActivatedRoute class ?

- [ ] `Both are Observables containing values from the requested route's URL string. The paramMap contains the parameter values that are in the URL path and the queryParamMap contains the URL query parameters`
- [ ] `paramMap is the legacy name from Angular 3. The new name is queryParamMap`
- [ ] `The paramMap is an object literal of the parameters in a route's URL path. The queryParamMap is an Observable of those`
- [ ] `The paramMap is an Observable that contains the parameter values that are part of a route's URL path. The queryParamMap is a method that takes in an array of keys and is used to find specific parameters in the paramMap`

#### Q26. When a service requires some setup to initialize its default state through a method, how can you make sure that said method is invoked before the service gets injected anywhere ?

- [ ] `Use a factory provider at the root AppModule level that depends on the service to call that service method`
- [ ] `Instantiate an instance of the service at the global level (window scope) and then call that method`
- [ ] `Put the logic of that service method into the service constructur instead.`
- [ ] `It is not possible to do it at application start; you can do it only at a component level`

#### Q27. What method is used to wire up a FormControl to a native DOM input element in reactive forms ?

- [ ] `Use the string name given to the FormControl as the value for the DOM element in reactive forms`
- [ ] `Use the formControlName directive and set the value equal to the string name given to the FormControl`
- [ ] `Add the string name given to the FormControl to an attribute named controls on the <form> element to indicate what fields it should include.`
- [ ] `Use the square bracket binding syntax around the value attribute on the DOM element and set that equal to an instance of the FormControl.`
   


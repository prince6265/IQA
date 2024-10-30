### Angular
- One of the popular javascript framework developed and maintained by Google. It is open-source framework based on Typescript Programming language. It's code is maintainable and reusable.

### some powerful features integrated into Angular
- It has some powerful feature like declarative template, end to end tooling, dependency Injection and various other best practices that smoothens the development path.

### Main Purpose of angular.
- Create fast, dynamic, and scalable web applications with the help of using components and directives.
- It supports dynamic content based on different users through dependency injection.
- YouTubeTV is the most popular example that uses Angular.
### Difference between Angular JS and Angular.
> AngularJS
- Version 
    - AngularJS was the very first version initially released in 2010. It was a browser-side JavaScript used within HTML code and created a revolution in web application development. It is popularly known as AngularJS.
- Architecture
    - AngularJS support the MVC Architecture.
- Supported Language.
    - JavaScript
- Expression syntax
    - In AngularJS, a specific ng directives are required for the image/property and events.
- Mobile Support
    - Angular js does not support mobile application.
- Dependency Injection  
    - AngularJS does not support dependency injection.
- Routing
    - In AngularJS, $routeprovider.when() is used for routing configs.
- structure
    - it is first and basic version of Angular so it is very easy to manage.
- Speed
    - Slower because of it's limited features.
> Angular
- Version
    - The later Angular versions were a complete rewrite of AngularJS. For example, Angular 2 was initially released in 2016. There is nothing common between Angular2 and AngularJS except the core developer's team.
    - After that, Angular 6, Angular 7, Angular 8, Angular 9, and Angular 10 were released that are very similar to each other. These later versions are known as Angular.
- Architecture
    - Angular uses components and directives
- Supported Language
    - typescript
- Expression syntax
    - Angular uses () fro event binding and [] for property binding.
- Mobile Support
    - It provide mobile support
- Dependency Injection
    - Angular supports hierarchical Dependency Injection ( components and services are organized in a tree structure. Each component can access dependencies (like services) from its parent and pass them down to its children. If a service needs to be shared across the entire application, it can be provided at the root level, but if it’s only needed for specific components, it can be defined at that component level. This makes memory usage efficient and keeps the code organized.) with uni-directional tree-based change detection.
- Routing
    - you define routes with the RouterModule. Each route maps a URL path to a specific component.
- structure 
    - It has a very simplified structure that makes the development and maintenance of large applications very easy.
- Speed 
    - It is faster than AngularJS because of its upgraded features.
- Support 
    - It provides active support, and frequent new updates are made.
### biggest advantages of using Angular?
- Angular supports two-way data-binding.
- It follows MVC pattern architecture.
- It supports static templates and Angular template.
- It facilitates you to add a custom directive.
- It also supports RESTfull services.
- Validations are supported in Angular.
- Angular provides client and server communication.
- It provides support for dependency injection.
- It provides powerful features like Event Handlers, Animation, etc.
### Angular expressions:
- Expressions are code snippets that are used to bind application data to HTML elements. usually written in double braces {{Expression}} like javascript.
### Templates in Angular:
- it contains angular specific elements attributes. these are written with html and combined with information coming from the model and controller, which are further used to provide dynamic view to the user.
### difference between an Annotation and a Decorator in Angular:
- Annotations and Decorators are both used to add metadata to classes, but they serve distinct purposes and have different origins. 
- Annotations are the "only" metadata set of the class using the Reflect Metadata library. They are used to create an "annotation" array.
- Decorators are the design patterns used for separating decoration or modification of a class without actually altering the original source code.
### Work flow of Angular Application:
1. App Initialization:
- Entry Point: The application starts from a main file (typically main.ts), which bootstraps or loads the root Angular module (AppModule).
- Root Module: AppModule contains essential setup and imports, and it launches the root component (AppComponent), the main view of the application.
2. Modules and Components:
- Modules: Angular apps are organized into modules, with each module grouping related components, services, and other functionality.
- Components: Components are building blocks for the UI. 
- Each component has:
    - A template (HTML) for structure.
    - Styles (CSS/SCSS) for design.
    - Logic (TypeScript) for handling data and interactions.
3. Data Binding and Interaction:
- Data Binding: 
    - This connects the UI and data, allowing you to:
    - Show dynamic data with interpolation ({{ data }}).
- Sync data between the UI and component with two-way binding.
- Event Binding: Links actions (like clicks) from the user to functions in the component.
- Property Binding: Updates the view automatically when the data changes.
4. Routing:
- Navigation: Angular’s router manages navigation between different parts (views) of the app.
- Routes: Defined in a routing module, specifying each URL and the component to display when that URL is visited.
5. Services and Dependency Injection:
- Services: Services handle shared data or logic that doesn’t belong to one specific component, like making API calls.
- Dependency Injection (DI): Angular uses DI to manage and inject services where they’re needed, such as in components that require data fetching.
6. HTTP Requests and APIs:
- HTTPClient Module: To interact with APIs, Angular uses the HttpClient module, allowing components to fetch or send data to a backend server.
- Observables: These allow handling async data (like data from an API) efficiently.
7. Change Detection:
- Angular automatically tracks changes in data and updates the UI accordingly using change detection. This makes sure that the view is always up-to-date with the data in the components.
8. Compilation and Optimization:
- Development Build: While coding, Angular runs a development build that helps catch errors and updates instantly.
- Production Build: When the app is ready, a production build optimizes it by minimizing file sizes and improving performance before deployment.
9. Deployment:
- The final build is deployed to a web server, making the app available to users.
### AOT in Angular:
- AOT(Ahead of time compiler) used to convert your angular HTML and typescript code into efficient javascript code during the build phase before the browser downloads and runs that code. 
- By compiling the application during the build process provides a faster rendering in the browser.
### reason for using the AOT compiler in Angular:
- An Angular application is made of several components and their HTML templates. 
- Because of these Angular components and templates, the browsers are not able to understand them directly. So, Angular applications require a compilation process before they run in a browser.
### advantages of AOT in Angular:
- The rendering is faster.
- The Angular framework's download size is smaller.
- Fewer asynchronous requests.
- Detect template errors earlier.
- Better security.
### What is JIT in Angular?
- JIT (Just-in-Time) compilation in Angular is a way to convert your Angular code (written in TypeScript and HTML) into JavaScript code while the app is running in the browser.
### difference between JIT and AOT in Angular:
- Just-in-Time (JIT) compiler compiles our app in the browser at run-time while Ahead-of-Time (AOT) compiler is used to compile your app at build time on the server.
- The JIT compilation runs by default when you run the ng build (build only), or ng serve (build and serve locally) CLI commands. This is used for development. On the other hand, we have to include the --aot option with the ng build or ng serve command for AOT compilation.
- JIT compiler is used in development mode while AOT is used for production mode.
- JIT is easy to use. We can easily implement features and debug in JIT mode because here we have a map file while AOT does not. On the other hand, the biggest advantage of using AOT for production is that it reduces the bundle size for faster rendering.
### concept of scope hierarchy in Angular?
- Angular provides the $scope objects into a hierarchy that is typically used by views. This is called the scope hierarchy in Angular. It has a root scope that can further contain one or several scopes called child scopes.
- In a scope hierarchy, each view has its own $scope. Hence, the variables set by a view's view controller will remain hidden to other view controllers.
### difference between Observables and Promises in Angular?
- In Angular, as soon as we make a promise, the execution takes place, but this is not the case with observables because they are lazy. It means nothing happens until a subscription is made.
- Promise
    - It emits a single value.
    - Not Lazy
    - We can not cancel it.
- Observable
    - It emits multiple values over a period of time.
    - Lazy. An observable is not called until we subscribe to the observable.
    - We can cancel it by using the unsubscribe() method.
    - Observable provides operators like map, forEach, filter, reduce, retry, retryWhen etc.
### directives in Angular:
- directives are special instructions added to the HTML to alter the DOM (Document Object Model) or change the appearance and behavior of elements.
> three main directives angular have
1. Component directive
      - These are the most common type of directive.
      - Components are essentially custom elements with their own templates, styles, and logic.
      ```TypeScript
      @Component({
          selector: 'app-hello',
          template: '<h1>Hello, World!</h1>'
        })
        export class HelloComponent {}
      ```
2. structure directive
      - Structural directives alter the DOM layout by adding or removing elements.
      - They use an asterisk (*) before their name in the template.
      - Common examples include *ngIf, *ngFor, and *ngSwitch.
3. attribute directive
      - Attribute directives change the appearance or behavior of an element without altering the DOM structure.
      - They look like regular HTML attributes but are used to dynamically change properties.
      - Common examples include ngClass, ngStyle, and custom attribute directives.
### Angular CLI?
- It is a command-line interface to scaffold and build angular apps using node.js style modules.
```powershell
npm install -g @angular/cli@18 
```
### Lazy loading Angular
- It is a concept of angular routing.
- it makes downloading data in chunks not in a single bundle.
- Lazy loading facilitates asynchronously loading the feature module for routing whenever required using the property loadChildren.
### router imports:
- The Angular Router, representing a particular component view for a given URL, is not part of Angular Core. It is available in a library named @angular/router, and we have to import the required router components. This process is called router imports.
```TypeScript
import { RouterModule, Routes } from '@angular/router';
```
### RouterOutlet and RouterLink:
- A RouterOutlet is a directive from the router library that acts as a placeholder. 
- It marks the spot in the template where the Router should display the components for that outlet. Router outlet is used as a component.
```HTML
<router-outlet></router-outlet>  
```
- On the other hand, a RouterLink is a directive on the anchor tags that gives the router control over those elements. Since the navigation paths are fixed, you can assign string values to router-link directive as below,
```HTML
<h1>Angular Router</h1>  
<nav>  
  <a routerLink="/todosList" >List of todos</a>  
  <a routerLink="/completed" >Completed todos</a>  
</nav>  
<router-outlet></router-outlet>
```
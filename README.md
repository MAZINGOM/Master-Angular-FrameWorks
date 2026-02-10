# Master-Angular-FrameWorks
Latest Angular Updates , Interview Questions , Angular tasks for hands on , E-commerce Project

1.Standalone components

@Component({
  selector: 'app-user-profile',
  standalone: true,
  imports: [CommonModule, ReactiveFormsModule],
  template: `<div>{{ user.name }}</div>`,
})
export class UserProfileComponent {}   

This simplifies the component structure & improves modularity.By default every component in Angular is  a standalone component
if we do not want a component to be a standalone ; we specify a flag named  standalone & set it to false .

2. Improved Dependency Injection
3. (inject() Function) In the newer version - Angular makes use of the inject() function -
   which allows dependency injection without  using constructors  making services & dependeincies more flexible with the standalone component.
   Earlier we used to inject the dependencies using the contructor.
   Constructor(private http:HttpClient) {}
   But now - we can directly user the inject() function to inject any dependency
   private http = inject(HttpClient);
   Not Only that , the dependency injection is more type refined .
   Constructor(private http:HttpClient) {}
   The compiler will infer the dependency as the type streamlining code & minimizing repetitive type declarations , the reduces the boilerplate & improves saftey in the code
4. Signal-Based Reactivity Model
   Angular has improved & enhanced its signal system for reactive programming
   import {signal } from '@angular/core'
   export class CounterComponent {

   counter = signal(0);
   increament() {
   this.counter.set(this,counter() + 1):
   }
   }
   it is now production-ready , providing a streamlined approach to state management - which basically involves the change detection of the states
   Now , we can easily manage state changes with reactive programming , using signals to make it simpler & less complicated
4. Optimized Preloading strategies
   slow loading times can lead to a frustrating user experince & ultimately drive users away .
   Angular 19 improves preloading with better strategies like enhanced PreloaAllMOdules & Custom Preloading Strategies
   provideRouter (routes , withPreloading(PreloadAllModules)),
   provideRouter (routes , withPreloading(CustomPreloadStrategy)),
   {
        path: 'second',
        loadComponent: () =>  
        import(./second/second.component').then((m) => m.SecondCompoent),
        data: {preload:true}
   },

5. Improeved Token Injection 
   Angular 19 introduces improvements for token injection with better support for tokens like useValue & useFactory .
   @Component ({
      prividers : [{
      useValue: {
         apiUrl: 'https://api.standalne-example.com',
         featureEnabled:true,

}as AppConfig,
},]})


& any such updates ...
6.Server-side rendering 
7. Client side hydration
8.Overall performance improvements

   }
   
   
   

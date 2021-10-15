# Observables Exercise
## Use Git or GitHub Desktop to push each exercise to GitHub


1. **Subscribe to the params observable and log the data to the console**

-   Generate a new angular application called basic-observable-example
    -   enable routing and make sure it is in non-strict mode
-   Generate a users component
-   In the app-routing module, create a path such as ```"users/:id"```, it's component will be te users component
-   Include the router outlet in the app.component.html because the root path starts in the app component.
-   Every time you enter "localhost:4200/users/1", you should be able to see the users component template rendered onto the page. 
-   Inject ActivedRoute to the users component.
    -   With it's reference, subscribe to the observable that is params and log to the console its data.
-   If you enter "localhost:4200/users/1" to the url search bar, you should be able to see an object that is log to the console such as ```{id: 1}```

2. **User pipe and map to manipulate the data the observable passes through**
   
- 
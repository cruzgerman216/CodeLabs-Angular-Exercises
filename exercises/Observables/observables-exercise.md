# Observables Exercise
## Use Git or GitHub Desktop to push each exercise to GitHub
## Enable routing and non-strict mode for all projects

1. **Subscribe to the params observable and log the data to the console**

- Generate a new angular application called basic-observable-example
- Generate a users component
- In the app-routing module, create a path such as ```"users/:id"```, it's component will be set to the users component
- Include the router outlet in the app.component.html because the root path starts in the app component.
- Every time you enter "localhost:4200/users/1", you should be able to see the users component template rendered onto the page. 
- Inject ActivedRoute to the users component.
    - With it's reference, subscribe to the observable that is params and log to the console its data.
- If you enter "localhost:4200/users/1" to the url search bar, you should be able to see an object that is log to the console such as ```{id: 1}```

2. **User pipe and map to manipulate the data the observable passes through**
   
- Generate a new angular application called basip-pipe-map-example
- Generate a foods component
- In the app-routing module, create a path such as ```"foods/:search"```, it's component will be set to the foods component.
- Include the router outlet in the app.component.html
- Inject ActivedRoute to the users component
  - subscribe to the params observable
  - store it's data in a class property called foodSearch that is of type string.
  - Use string interpolation to output the foodSearch class property onto the web page
- If you enter "localhost:4200/foods/pie", you should get the text "pie" on the webpage
- Use pipe and the map operator to manipulate the data. Instead of returning an object, return a string that has "the food you search for was " followed by what the user search for. Make sure whatever the user search for, is capitlized when you return the manipulated data. Example: "The food you search for was Pie".
- If you enter "localhost:4200/foods/pie", you should get the text "The food you search for was Pie" and rendered onto your webpage.

3. **Use filter to manipulate data of an interval observable and the unsubscribe method to destroy the subscription**
- Generate a new angular application called interval-filter-example
- generate a home and timer component and create it's corresponding routing paths "home" and "timer"
- In app.component.html, include elements with routlinkers to each component so you can switch between both paths. Of course, add the router link element 
- In timer.component.ts, import interval from rxjs and use it to increment a number every second. Log to the console the incremented number
- Make sure you unsubscribe from the observable. To make sure you did this right, switch between the paths. If you are in the home path, you shouldn't see anything log to the console.
- Use the filter operator to pass only even numbers

    Reference: https://rxjs.dev/api/index/function/interval

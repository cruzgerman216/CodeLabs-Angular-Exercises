# Observable Exercises
### Use Git or GitHub Desktop to push each exercise to GitHub
### Enable routing and non-strict mode to all projects

**Exercise 1: Subscribe to the params observable and log the data to the console**
- Generate a new angular application called basic-observable-exercise
- Generate a users component
- In the app-routing module, create a path such as ```"users/:id"```, it's component will be set to the users component
- Include the router outlet in the app.component.html because the root path starts in the app component.
- Every time you enter "localhost:4200/users/1", you should be able to see the users component template rendered onto the page. 
- Inject ActivedRoute to the users component.
    - With it's reference, subscribe to the observable that is params and log to the console its data.
- If you enter "localhost:4200/users/1" to the url search bar, you should be able to see an object that is log to the console such as ```{id: 1}```

**Exercise 2: User pipe and map to manipulate the data the observable passes through**
- Generate a new angular application called basic-pipe-map-exercise
- Generate a foods component
- In the app-routing module, create a path such as ```"foods/:search"```, it's component will be set to the foods component.
- Include the router outlet in app.component.html
- Inject ActivedRoute to the foods component
  - subscribe to the params observable
  - access the object's search property, store it's value in a class property called foodSearch that is of type string. 
  - Use string interpolation to output the foodSearch class property onto the web page
- If you enter "localhost:4200/foods/pie", you should get the text "pie" on the webpage
- Use pipe and the map operator to manipulate the data. Instead of returning an object, return a string that has "the food you search for was " followed by what the user search for. Make sure whatever the user search for, is ALL UPPER CASE when you return the manipulated data. Example: "The food you search for was PIE".
- If you enter "localhost:4200/foods/pie", you should get the text "The food you search for was PIE" and rendered onto your webpage.

**Exercise 3: Use filter to manipulate data of an interval observable and the unsubscribe method to destroy the subscription**
- Generate a new angular application called interval-filter-exercise
- generate a home and timer component and create it's corresponding routing paths "home" and "timer"
- In app.component.html, include elements with routlinkers to each component so you can switch between both paths. Of course, implement the router link element to the application
- In timer.component.ts, import interval from rxjs and use it to increment a number every second. Log to the console the incremented number
- Make sure you unsubscribe from the observable. To make sure you did this right, switch between the paths. If you are in the home path, you shouldn't see anything log to the console.
- Use the pipe method and the filter operator from rxjs to pass only even numbers

    Reference: https://rxjs.dev/api/index/function/interval

**Exercise 4: Instead of an EventEmitter, use a subject to emit data.**
Note: Using an event emitter in services is bad practice. Instead, use subjects
- Generate a new angular project called basic-subject-exercise
- Generate a navbar component, 
  - in the navbar.component.html file, include an input element and a button with content "Print my text!"
  - use two way data binding to store the value of whatever the user type in a class property called search of type string and that is initially empty.
  - Whenever you click on the button, log to the console the search property
- Create a service file called data.service.ts, and set a class property called mySearch to a new Subject.
- Inject the data service to the navbar component, and use the next method to emit the search property. Whenever you click the button, you want to execute this next method.
- Inject the data service class to the app component, subscribe to the mySearch property and store it's emitted data into a property called searchResult of type string  and set initally set it to empty. 
- Use string interpolation to output the value of searchResult to the app.component.html
- Use the pipe method and filter operator to filter out any searches that equal "hat"
- Use the map operator to adjust the data to "You searched for " followed by whatever the user searches for
- Unsubscribe from the subject in the app.component.ts file
    - Note: App.componen.ts is never destroyed but just for practice, do this anyways.

**Exercise 5: More Subjects**
[Github Repo Starting Code](https://github.com/WilderDev/Candy-Observables-Project/tree/Starter-Code)
1. Create a new Subject in the PillowCaseService that emits when the myCandies array updates.
2. Subscribe to that change and update the local myCandies array.
3. Create a variable of type "Subscription", store the observable under inside, and use ngOnDestroy to unsubscribe when the component is destoyed.
4. Create a new Subject in the CandyStoreService that emits when the candiesForSale array updates.
5. Subscribe to that change and update the local candiesForSale array.
6. Create a variable of type "Subscription", store the observable under inside, and use ngOnDestroy to unsubscribe when the component is destoyed.
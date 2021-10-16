# Components & Databind Deep Dive Exercise
### Use Git or GitHub Desktop to push each exercise to GitHub
### Make projects all non-strict mode

1. **Allow a child component to recieve values from the parent component using the input decorator**
 - Create a new angular project called basic-custom-property-exercise
 - Generate a component called user, nest user in the app component
 - In app.component.ts, create a class property called name of type string and set it to your name.
 - In the user.component.ts file, create a class property called myName of type string and set it initially to be empty. Configure this property by the @Input Decorator.
   - Use string interpolation to output the name of myName onto the webpage.
 - In app.component.html, pass down the name property to the user component.
 - run 'ng serve' and you should see your name on the webpage.

2. **Passing down information two levels deep using the input decorator**
 - Create a new angular project called nested-components-input-exercise
 - Generate two components called myprofile and posts
 - myprofile should be nested in the component and posts should be nested in the myprofile component
 - In the app.component.ts file, create a class property that is called myPosts that is of type array of strings and set it to an array of pre-filled strings.
 - Pass down myPosts to the myprofile component, and make myprofile pass that down to the posts component.
 - In posts.component.ts, use ngFor to output the array of strings.
 - run 'ng serve' and you should see a list of strings you addded to the myPosts array.

3. **Use ngFor and the input decorator to allow the parent component to pass down information to the child component**
  - Create a new angular project called ngFor-input-decorator-exercise
  - generate a component called user and nest it in the app component
  - In app.component.ts, create a class property called users that is an array of type object. The object must contain properties user of type string, id of type number. Fill the array with these objects.
  - Use ngFor to pass each element of the property users value to the user component.
    - NOTE: For example, the user component must incorporate a property called for example, user_info that is configured by the input decorator.
  - Give the property that is configured by the input decorator an alias of "inputUser"
  - Output the user_info in user.component.html, using string interpolation and add an h1 element that has the content "User info!".
  - run 'ng serve' and you should see a list of users and numerous h1 elements.

4. **Use a custom event to pass information to the parent component**
  - Create a new angular project called basic-custom-event-exercise
  - Generate a component called navbar and nest it in the app component
  - In navbar.component.html file, create an input element and incorporate two way data binding or any way you like to store whatever the user type in a class property called mySearch. 
  - In navbar.component.ts, use an event emitter to emit the class property mySearch.
  - Configure app.component.html, to store that information that is being sent by navbar in a class property called searchResult.
  - Use string interpolation to output searchResult.
  




  

  
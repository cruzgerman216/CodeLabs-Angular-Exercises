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

2. **Use ngFor to loop through an array of elements, use the input decorator so that a child component can get the parent component's value**
  - Create a new angular project called ngFor-input-decorator-exercise
  - generate a component called user and nest it in the app component
  - In app.component.ts, create a class property called users that is an array of type object. The object must contain properties user of type string, id of type number. Fill the array with these objects.
  - Use ngFor to pass each element of the property users value to the user component.
    - NOTE: For example, the user component must incorporate a property called user_info that is configured by the input decorator.
  - Give the property that is configured by the input decorator an alias of "input
  - Output the user_info in user.component.html, using string interpolation
  
  
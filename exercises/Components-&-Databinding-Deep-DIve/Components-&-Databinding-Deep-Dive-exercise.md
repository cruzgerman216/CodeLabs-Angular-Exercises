# Components & Databind Deep Dive Exercise
### Use Git or GitHub Desktop to push each exercise to GitHub
### Make projects all non-strict mode

1. Use ngFor to loop through an array of elements and output their values
  - Create a new angular project called basic-custom-property-example
  - generate a component called user and nest it in the app component
  - In app.component.ts, create a class property called users that is an array of type object. The object must contain properties user of type string, id of type number. Fill the array with these objects.
  - Use ngFor to pass each element of the property users value to the user component.
    - NOTE: the user component must incorporate a property called user_info that is configured by the input decorator.
  - Output the user_info in user.component.html, using string interpolation
  
  
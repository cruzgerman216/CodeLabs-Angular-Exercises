
# The Basics Exercises
### Use Git or GitHub Desktop to push each exercise to GitHub
### Make projects all non-strict mode

**Exercise 1: Manually create a component**
  - create a new angular project called manually-create-component
  - without using the angular cli to generate a component, manually create a 
   component called home.
  - inside of the home template, create a paragraph tag with content "I'm home!" 
  - the home component should be nested in the app component.
  - "I'm home" should be displayed onto the webpage when you run 'ng serve'

**Exercise 2: Generate a component**
  - create a new angular project called generate-angular-component
  - using the angular cli, generate a component called post
  - inside of the post's template, create a div element with the content "I'm a post!"
  - the post component should be nested in the app component.
  - "I'm a post!" should be displayed onto the webpage when you run 'ng serve'

**Exercise 3 Manually create a component and style it**
  - create a new angular project called manually-create-component-style
  - without using the angular cli to generate a component, manually create a 
   component called paragraph-list.
  - inside of the paragraph-list template, create multiple paragraph elements with content
  - the paragraph-list component should be nested in the app component
  - use the paragraph-list.component.css, create a couple of css classes to change the background color or the text color
  - of each paragraph element
  - run 'ng serve' in the terminal and each paragraph element should have a change of style

**Exercise 4: Create multiple components**
  - create a new angular project called create-multiple-components
  - manually create or use the angular CLI to generate two components: navbar and home
  - edit the navbar's component template(navbar.component.html), create a paragraph element with content "I'm the navbar!"
  - edit the home's component template(home.component.html), create a paragraph element with content "I'm the home!"
  - display each component in the app component
  - run 'ng serve' in the terminal and you should see both paragraph tags

![alt text](/assets/images/1-the-basics/1.png)

**Exercise 5: Create nested components**
  - create a new angular project called create-nested-components
  - generate three components: child-one,child-two,child-three
  - edit child-one's template, create a paragraph element with content "I'm the app component's child!"
  - edit child-two's template, create a paragraph element with content "I'm child-one's child!"
  - edit child-three's template, create a paragraph element with content "I'm the child-two's child!"
  - nest childone into app component
  - nest childtwo into childone
  - nest childthree into childtwo
  - run 'ng serve' in the terminal and you should see each components template rendered onto the webpage.

![alt text](/assets/images/1-the-basics/2.png)

**Exercise 6: Create complex structure components**
  - create a new angular project called create-complex-structure
  - Generate a component structure that looks similiar to the diagram
  - run 'ng serve' in the terminal and you should see each components template rendered.
  ![alt text](/assets/images/1-the-basics/3.png)

**Exercise 7: Use string interpolation to output content to the webpage**
  - create a new angular project called string-interpolation-exercise
  - create a property in app.component.ts called "name", set it's type to string and make it equal to your name(for exercise: "John")
  - create a paragraph element and use string interpolation to output the value of name.
  - run 'ng serve' in the terminal and you should see your name on the webpage.


**Exercise 8: Use string interpolation to output the values an object holds**
  - create a new angular project called string-interpolation-object
  - generate a component called post
  - nest the post component in app component
  - In app.component.ts, create a class property called heading with a type string and set it equal to "user post".
  - In app.component.ts, create a class property called num with a type number and set it equal to 1. 
  - In the app.component.html file, create a h1 elmeent with the content of both class properties heading and num.
  - in the post.component.ts, create a class property called 'info' that is an object with properties: firstname, lastname, content. Fill in the values for these properties
  - use string interpolation to output these properties values from the object. 
  - run 'ng serve' in the terminal to see the values of the object onto the page, also heading,num.

**Exercise 9: Use a ternary operator to dynamically output content**
  - create a new angular project called ternary-operator-string-interpolation.
  - generate a component called navbar and nest it in the app acomponent
  - In navbar.component.ts, create a property called loggedIn with type boolean and set it equal to true;
  - In navbar.component.html, create a div element, in the div element, use string interpolation to output "I am logged in!" if the loggedIn class property is true, otherwise output "I am logged out!". 
  example of ternary operator: true ? "output me if true" : "output me if false"

**Exercise 10: Use property binding to disable an input element**
  - create a new angular project called basic-property-binding
  - In app.component.ts, create a class property called isDisabled with type boolean and set it equal to true
  - In app.component.html, create an input element and use property binding to bind the html attribute disabled(see reference of what it is) to the set class property isDisabled.
  - run 'ng serve', if it works, you shouldn't be able to type anything in the input field
  - now set isDisabled to false then run 'ng serve', you should be able to type in the input field.

Reference: https://www.w3schools.com/tags/tag_input.asp

  **Exercise 11: Use property binding to adjust the height and width of an image.**
  - create a new angular project called property-binding-image-size
  - In app.component.ts, create two class properties called width and height. Both properties have type number and a value between 100 - 500 (you choose the number)
  - In app.component.html, create an img element(see reference of an exercise) and include it's src attribute. Copy an image address link from google (make sure it has an image extension at the end of the link) and set src to the image link. 
  - now add two more attributes: width and height and use property binding to set it to the class properties you made in your app.component.ts file.

Reference: https://www.w3schools.com/tags/att_height.asp

   **Exercise 12: Click on a button to log to the console a message**
  - Create a new angular project called basic-event-binding-exercise
  - In app.component.html, create a button element with content "Click me to log to the console!"
  - Implement event binding to the button element you created so that, whenver you click the button, it logs a message(could be anything) to the console.
  - run 'ng serve' and click on the button. You should be able to see something output to the console in the dev tools of your browser.

  **Exercise 13: Dynamically disable and enable the input field using event binding and property binding.**
  - Create a new angular project called dynamic-button-event-binding
  - In app.component.ts, create a class property called isDisabled of type boolean and set it to true.
  - In app.component.html, create an input element and incorporate property binding by disabling or enabling the input element depending on the value of the class property isDisabled. 
  - Create a button element with content "Click me to change the value of isDisabled!"
  - Use event binding for whenever you click te button, you set isDisabled to the opposite of it's current value.
example: If isDisabled is true
        when I click on the button, isDisabled is set to false.
  - In the button element content, it currently has "Click me to change the value of isDisabled!", use the ternary opperator and string interpolation to be able to output "Currenlty disabled" when the isDisabled property is true, and vice versa for when it's false.
  - run 'ng serve'. You should be able to type into the input field when isDisabled is false and vice versa for when it is true.

  **Exercise 14: Use ngModel to dynamically change the value of a class property**
  - Create a new angular project called basic-ngmodel-exercise
  - In app.component.ts, create a class property called title of type string and set it equal to "header"
  - In app.component.html, create an h1 element and use string interpolation to output the value of the class property header.
  - Create an input element that implements two way data binding, ngModel, that will dynamically change the value of header for whenever you type into the input field.
  - run 'ng serve' to confirm this works.

  **Exercise 15: Dynamically change the value of a class property without using ngModel**
  - Create a new angular project called input-event-binding-exercise
  - In app.component.ts, create a class property called title of type string and set it equal to "header"
  - In app.component.html, create an h1 element and use string interpolation to output the value of the class property header.
  - Create an input element that implements event binding and property binding to get the same effect of ngModel
Notes: You will need to use attributes ```input``` for event binding and ```value``` for property binding

Reference: 
https://www.w3schools.com/tags/att_input_value.asp -> learn what ```value``` does to an input element
You can incorporate event binding to any event listener onClick,onMouseenter, OnInput(https://www.w3schools.com/jsref/dom_obj_event.asp)

The specific event listener we want to use is ```input```, every time the user types, input will trigger an event. Be sure to use the $event to get it's value. log to the console the value. You will see that event.target.value will get you whatever the user type.

```html
  <input (input)="">
```

  **Exercise 16: Use ngIf and a class property to show the element, if the class property is false, it shouldn't show the element**
  - Create a new angular project called basic-ngif-exercise
  - In app.component.ts, create a class property called isShow of type boolean and set it to true.
  - In app.component.html, create a paragraph element with the content of "Show me when isShow is true! Otherwise, don't show me!"
  - Use ngIf to conditionally show the paragraph element for when isShow is true, otherwise don't show it if it's false.
  - run 'ng serve', isShow is set to true so you should see your paragraph element there.
  - Set isShow to false, and it shouldn't show in the webpage.

  **Exercise 17: Use ngIf and else to dynamically add certain elements to the webpage**
  - Create a new angular project called basic-ngif-else-exercise
  - In app.component.ts, create a class property called isShowContent of type boolean and set it to true
  - In app.component.html, create a paragraph element with content "If isShowContent is true, show me!" and
  another paragraph with content "Use else to show me!"
  - use ngIf and else to show either or depending on the value of isShowContent.
  - Create a button element with content "Click me to reverse the value of isShowContent!" Use event binding to reverse the value of isShowContent.

  **Exercise 18: Use ngStyle to change the background color of an element**
  - Create a new angular project called basic-ngStyle-exercise
  - In app.component.ts, create a class property called myColor of type string and set it to "green"
  - In app.component.html, create a paragraph element with content "This should change when we implement ngStyle!" 
  - Implement ngStyle and use myColor to change the background color of the paragraph element.
  - run 'ng serve' The paragraph element should have background color of green.

  **Exercise 19: Use ngStyle and event binding to dynamically change the content of an element and it's style.**
  - Create a new angular project called dynamically-change-content-ngstyle-exercise
  - In the app.component.ts, create a class property called changeColor, make it of type string and set it to 'green'.
  - In app.component.html, create an input element. Whenever you type into this input field, it should dynamically change the value of changeColor to whatever you type. You can use either ngModel or event binding to do this.
  - Create a paragraph element. Use string interpolation to output the value of changeColor between the tags of the paragraph element.
  - Use ngStyle and changeColor to change the color of the content that the paragraph element holds.
  - run 'ng serve'. If you type in yellow, the color of the text should change to yellow.

  **Exercise 20:Use ngFor to output each element of an Array**
  - Create a new angular project called basic-ngFor-exercise
  - In app.component.ts, create a class property called foods, make it type array of strings and set its array to pre-set strings. 
  - In app.component.html, use ngfor to output the array list of foods
  - run 'ng serve' you should be able to see each element of the array on the web page



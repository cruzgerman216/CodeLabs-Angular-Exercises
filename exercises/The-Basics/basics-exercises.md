
# The Basics Exercise
## Use Git or GitHub Desktop to push each exercise to GitHub

1. Manually create a component
  - create a new angular project called manually-create-component
  - without using the angular cli to generate a component, manually create a 
   component called home.
  - inside of the home template, create a paragraph tag with content "I'm home!" 
  - the home component should be nested in the app component.
  - "I'm home" should be displayed onto the webpage when you run 'ng serve'

2. Generate a component
  - create a new angular project called generate-angular-component
  - using the angular cli, generate a component called post
  - inside of the post's template, create a div element with the content "I'm a post!"
  - the post component should be nested in the app component.
  - "I'm a post!" should be displayed onto the webpage when you run 'ng serve'

3. Manually create a component and style it
  - create a new angular project called manually-create-component-style
  - without using the angular cli to generate a component, manually create a 
   component called paragraph-list.
  - inside of the paragraph-list template, create multiple paragraph elements with content
  - the paragraph-list component should be nested in the app component
  - use the paragraph-list.component.css, create a couple of css classes to change the background color or the text color
  - of each paragraph element
  - run 'ng serve' in the terminal and each paragraph element should have a change of style

4. Create multiple components
  - create a new angular project called create-multiple-components
  - manually create or use the angular CLI to generate two components: navbar and home
  - edit the navbar's component template(navbar.component.html), create a paragraph element with content "I'm the navbar!"
  - edit the home's component template(home.component.html), create a paragraph element with content "I'm the home!"
  - display each component in the app component
  - run 'ng serve' in the terminal and you should see both paragraph tags

![alt text](/assets/images/1-the-basics/1.png)

5. Create nested components
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

6. Create complex structure components
  - create a new angular project called create-complex-structure
  - Generate a component structure that looks similiar to the diagram
  - run 'ng serve' in the terminal and you should see each components template rendered.
  ![alt text](/assets/images/1-the-basics/3.png)

7. Use string interpolation to output content to the webpage
  - create a new angular project called string-interpolation-exercise
  - create a property in app.component.ts called "name", set it's type to string and make it equal to your name(for example: "John")
  - create a paragraph element and use string interpolation to output the value of name.
  - run 'ng serve' in the terminal and you should see your name on the webpage.


8. Use string interpolation to output the values an object holds
  - create a new angular project called string-interpolation-object
  - generate a component called post
  - nest the post component in app component
  - In app.component.ts, create a class property called heading with a type string and set it equal to "user post".
  - In app.component.ts, create a class property called num with a type number and set it equal to 1. 
  - In the app.component.html file, create a h1 elmeent with the content of both class properties heading and num.
  - in the post.component.ts, create a class property called 'info' that is an object with properties: firstname, lastname, content. Fill in the values for these properties
  - use string interpolation to output these properties values from the object. 
  - run 'ng serve' in the terminal to see the values of the object onto the page, also heading,num.

9. Use a ternary operator to dynamically output content
  - create a new angular project called ternary-operator-string-interpolation.
  - generate a component called navbar and nest it in the app acomponent
  - In navbar.component.ts, create a property called loggedIn with type boolean and set it equal to true;
  - In navbar.component.html, create a div element, in the div element, use string interpolation to output "I am logged in!" if the loggedIn class property is true, otherwise output "I am logged out!". 
  Example of ternary operator: true ? "output me if true" : "output me if false"

10. Use property binding to disable an input element
  - create a new angular project called basic-property-binding
  - In app.component.ts, create a class property called isDisabled with type boolean and set it equal to true
  - In app.component.html, create an input element and use property binding to bind
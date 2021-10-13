
# The basics execise
## Use Git or GitHub Desktop to push each exercise to GitHub

1. Manually create a component
  - create a new angular project with the name of manually-create-component
  - without using the angular cli to generate a component, manually create a 
   component called home.
  - inside of the home template, create a paragraph tag with content "I'm home!" 
  - the home component should be nested in the app component.
  - "I'm home" should be displayed onto the webpage when you run 'ng serve'

2. Manually create a component and style it
  - create a new angular project with the name of manually-create-component-style
  - without using the angular cli to generate a component, manually create a 
   component called paragraph-list.
  - inside of the paragraph-list template, create multiple paragraph elements with content
  - the paragraph-list component should be nested in the app component
  - use the paragraph-list.component.css, create a couple of css classes to change the background color or the text color
  - of each paragraph element
  - run 'ng serve' in the terminal and each paragraph element should have a change of style

3. Create multiple components
  - create a new angular project with the name of create-multiple-components
  - manually create or use the angular CLI to generate two components: navbar and home
  - edit the navbar's component template(navbar.component.html), create a paragraph element with content "I'm the navbar!"
  - edit the home's component template(home.component.html), create a paragraph element with content "I'm the home!"
  - display each component in the app component
  - run 'ng serve' in the terminal and you should see both paragraph tags

![alt text](/assets/images/1-the-basics/1.png)

4. Create nested components
  - create a new angular project with the name of create-nested-components
  - generate three components: child-one,child-two,child-three
  - edit child-one's template, create a paragraph element with content "I'm the app component's child!"
  - edit child-two's template, create a paragraph element with content "I'm child-one's child!"
  - edit cihld-three's template, create a paragraph element with content "I'm the child-three's child!"
  - nest childone into app component
  - nest childtwo into childone
  - nest childthree into childtwo
  - run ng serve in the terminal and you should see each components template rendered onto the webpage.

![alt text](/assets/images/1-the-basics/2.png)

5. Create complex structure components
  - create a new angular project with the name of create-complex-structure
  - Generate a component structure that looks similiar to the diagram
  - run ng serve in the terminal and you should see each components template rendered.
  ![alt text](/assets/images/1-the-basics/3.png)


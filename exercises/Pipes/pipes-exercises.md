# Pipe Exercises
### Use Git or GitHub Desktop to push each exercise to GitHub
### Enable routing and non-strict mode to all projects

## You can use one project for all exercises

 **Exercise 1.1: Use a pipe function to uppercase the value of a property**
- Generate a new angular application called basic-pipe-exercies
- create a property called name of type string and set it to your name;
- Use string interpolation to output the value of name to the webpage
- Use a pipe function to uppercase the value of name.

reference: https://angular.io/api/common/LowerCasePipe

 **Exercise 1.2: Currency in EURos and using a pipe parameter**
- create a property called wallet of type number and set it to 50.04;
- Use string interpolation to output the value of wallet onto the webpage
- Use a currency pipe function to change the output of the wallet property into dollar amounts.
- By default, it'll give you a USD symbol. Use the reference provided below as a guide to change the symbol from USD to European currency. 
reference: https://angular.io/api/common/CurrencyPipe

**Exercise 1.3: Create your own custom lowercase pipe**
- Create a property called sentence of type string and set it to "I went to go watch the Spiderman movie with my aunt May."
- Use string interpolation to output the value of sentence onto the webpage
- Manually create a custom pipe called 'mylowercasepipe' without the angular CLI and apply the pipe to the sentence value to transform its data to all lower case. Use the reference to help you do that.
- When you run 'ng serve' you should get "i went to go watch the spiderman movie with my aunt may."

reference: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/toLowerCase

**Exercise 1.4: Transform data that holds a string with more than X characters**
- Create a property called loremSentence of type string and set it to "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. "
- Use string interpolation to output the value of loremSetence onto the webpage
- Generate a pipe using the cli ```ng g p pipename``` called xAmountOfCharacters. When applied to the loremSentence, make it so that only the first x amount of characters will show followed by "...". Use a pipe parameter to set x. 

For example if you set x to be 5, then your output should be 
```Lorem...```

**Exercise 1.5: Create a filter pipe that's filters an array**
- Create a property called petThoughts of type string and set it to 
```['Cats are awesome.', 'Cats are sneaky.', 'Cats and dogs are both amazing!', 'Dogs are great.', 'Dogs are hyper.']```
    - use ngfor to output the elements of petThoughts
- Create an input element and use two way data binding to capture whatever the user type and put it into a class property called filterResults of type string set to ''
- Generate a custom pipe called filterPets and make it so you are able to filter through the array petThoughts. You will need to set up a parameter to be able to keep track of what the user type. Use the reference to check whether the string starts with filteredResults.

- run 'ng serve', when you type 'Cats' into the input field, you should see
   Cats are awesome. 
   Cats are sneaky.
   Cats and dogs are both amazing!


Reference: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/startsWith

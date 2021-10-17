# Forms Exercise
### Use Git or GitHub Desktop to push each exercise to GitHub
### Enable routing and non-strict mode to all projects

1. **Log to the console form values using the template driven approach**
- Generate a new angular application called basic-template-driven-exercise
- In app.component.html, create a form element. Inside of the form element, create an input element alongside with a button element. Give the button element a type set to submit and content "submit".  Give the input element a name that is set to ```"username```
- Use the template driven approach to access the values from this form and log them to the console.

2. **Log to the console form values using the template driven approach**
- Generate a new angular application called another-basic-template-driven-exercise
- In app.component.html, create a form element. Inside of the form element, create an input element alongside with a button element. Give the button element a type set to submit and content "submit". Give the input element a name that is set to ```"firstname```. 
- Create another input and set it's name to ```"lastname"```
- Create another input and set it's name to ```"username"```
- Use the template driven approach to access the values from this form and log them to the console.

3. **Log to the console form values using the template driven approach and the ViewChild decorator**
- Generate a new angular application called viewchild-template-driven-exercise
- In app.component.html, create a form element. Inside of the form element, create an input element alongside with a button element. Give the button element a type set to submit and content "submit". Give the input element a name that is set to ```"city"```. 
- Use the template driven approach and @ViewChild to access the values from this form and log them to the console.

Example 
```typescript
@ViewChild('f') form:NgForm;
```

4. **Add validators to the form inputs**
- Generate a new angular application called basic-form-validators-exercise
- In app.component.html, create a form element. Inside of the form element, create an input element alongside with a button element. Give the button element a type set to submit and content "submit". Give the input element a name that is set to ```"username"```. 
- Add the required validator to the input element
- Use the template driven approach to log to the console the form's values.
- When you inspect the input element on the page, once the input field is empty, you should see invalid added onto the input element. Once you type into the field, you should see valid added onto the input element.
- 


5. **Implement a disabled button for when the form is invalid**
- Generate a new angular application called disabled-form-button-validators-exercise
- In app.component.html, create a form with input elements and a submit button.
- All input elements should be required.
- If the form is invalid, disable the submit button.
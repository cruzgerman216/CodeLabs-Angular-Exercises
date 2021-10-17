# Forms Exercise
### Use Git or GitHub Desktop to push each exercise to GitHub
### Enable routing and non-strict mode to all projects

1. **Log to the console form values using the template driven approach**
- Generate a new angular application called basic-template-driven-exercise
- In app.component.html, create a form element. Inside of the form element, create an input element alongside with a button element. Give the input element a name that is set to ```"username```
- Use the template driven approach to access the values from this form and log them to the console.

2. **Log to the console form values using the template driven approach**
- Generate a new angular application called another-basic-template-driven-exercise
- In app.component.html, create a form element. Inside of the form element, create an input element alongside with a button element. Give the input element a name that is set to ```"firstname```. 
- Create another input and set it's name to ```"lastname"```
- Create another input and set it's name to ```"username"```
- Use the template driven approach to access the values from this form and log them to the console.

3. **Log to the console form values using the template driven approach and the ViewChild decorator**
- Generate a new angular application called viewchild-template-driven-exercise
- In app.component.html, create a form element. Inside of the form element, create an input element alongside with a button element. Give the input element a name that is set to ```"city"```. 
- Use the template driven approach and @ViewChild to access the values from this form and log them to the console.

Example 
```typescript
@ViewChild('f') form:NgForm;
```


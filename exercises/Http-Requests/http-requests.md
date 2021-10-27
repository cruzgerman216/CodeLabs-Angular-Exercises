# HTTP Request Exercises
### Use Git or GitHub Desktop to push each exercise to GitHub
### Enable routing and non-strict mode
### You can use one project for all exercises

## Getting Started with HTTP requests exercises
 - Create a firebase project called movies-project
   - Refer to this markdown file on how to setup a firebase project 
reference: [Firebase Setup](https://github.com/cruzgerman216/CodeLabs-Angular-Exercises/blob/main/assets/resources/firebase-setup.md)


 **Exercise 1.1: Send a Post request to firebase to add movie data**
- Generate a new angular application called basic-angular-http-request-exercies
- Create an h1 element with content "My Movies"
- Create an h3 element with content "Add Movie"
- Create a form with inputs and labels corresponding to title and genre. Include a button with content 'create Movie'
  - Configure the form in the template driven approach or the reactive approach
    Note: Make sure you add the right modules to your app module. 
      FormsModule(Template driven)
      ReactiveFormsModule(Reactive)
- Create a post request that allows you to add an object with properties title and genre to the firebase database you created from the start
  - Make sure you Inject the HttpClient to your component AND import the HttpClientModule to your app module. Include HttpClientModule to your imports array.
```typescript 
import {HttpClientModule} from '@angular/common/http'
```
  - When making a request, make sure you include "movies.json" at the end of the URL
    Example: ```https://my-test580f1-default-rtdb.firebaseio.com/movies.json```
  - Be sure to use the subscribe method as you are dealing with an observable(in the subscribe method, you will get back a response, log the response to the console)
- When sending a post request, you should see the values you inputed in the form, saved to the database.

**Exercise 1.2: Send a get request to firebase to retrieve movie data**

- Create an h3 element with content "List of Movies"
- Create a button with content "retrieve movies" and incorporate event binding to execute a method called onRecieveMovies()
- In the onRecieveMovies method, make a get request to access the movie data from the firebase database. 
- We want to ultimately get an array to output onto the webpage, however, we get an object as a response, use the pipe method and the map operator to change the response into an array. Refer to the reference as an example to access each value from the response. Of course, use console log the data as well to see what exactly is the response.

Reference: Example
```typescript
      for(const elem in data){
        myArray.push(data[elem])
      }
```
- In the subscribe method, store the data that is being passed in, in a property called myMovies which is set to any empty array initially;
- Use ngFor to output the array of myMovies. You should see the data that exists from firebase onto your webpage.
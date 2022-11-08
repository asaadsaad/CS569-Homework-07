# CS569 Homework
### Angular Router Module and Guards
**Update the previous Homework:**
  
* Add Angular Router module
* Remove the Show/Hide button and convert `AppComponent` into a template with a router link to navigate to `UsersComponent` when `/users` is requested.  
  
**Extra Requirements:**
* Update `UserComponent` to display a button on each card, when it's clicked it navigates to (`/user/:email`) and passes the user object through the navigation state.
* Create a new component `UserDetailsComponent` mapped to `/user/:email`, the component receives the full `User` object from the navigation state and displays more details about the user. Add a back button that goes to `/users`.
* If a user tried to visit `UserDetailsComponent` without passing a correctly formatted `:email`, your app will redirect them to a friendly error page. (use Guards)


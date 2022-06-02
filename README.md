# CS569 Homework 06
### Angular Router Module and Guards
**Update the previous Homework:**
* Add Angular Router module
* Remove the Show/Hide button and convert `AppComponent` into a template with a link to `UsersComponent`.
* Update `UsersComponent` so it saves the users list in a global state.
* When we navigate to `/users/, the application shows the cards.
* Add a button to each card so when we clicked it goes to (`/users/:email`), create a new `UserDetailsComponent` to display more details.
* If a user tried to visit `UserDetailsComponent` without passing an `:email` or passes a wrong `:email`, then your app will redirect them to a friendly error page. (use Guards)


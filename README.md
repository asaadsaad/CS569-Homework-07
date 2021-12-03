# CS569 Homework 07
### Angular Router Module and Guards
**Update the previous Homework:**
* Add Angular Router module and convert your `AppComponent` into a template.
* When we navigate to `/users/, the application shows list of users (first and last name only) by default (`UsersComponent`).
* When we click on a user (`/users/:email`), show a card of the user other details (`UserComponent`) within the `UsersComponent` as a child route.
* If a user tried to visit `UserComponent` without passing an `id` or passes a wrong `id`, then your app will redirect them to a friendly error page. (use Guards)


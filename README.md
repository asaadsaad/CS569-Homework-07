# CS569 Homework 08
### Angular Router Module and Guards
* Create a service `db` that returns an observable with the following response:
```javascript
[{_id: 1, name:'Natural Prairie', produce:['lettuce', 'tomato']}, ...]
```
* Create a component `farmersMarket` that is responsible for showing the farm name and types of produce.
```html
<ul>
  <li><a href="/farm/1">Natural Prairie</a></li>
  ...
</ul> 
```
* When users click on a farm name link you should direct them to a `farmDetails` child component that shows full details about the farm.
* If a user tried to visit `farmDetails` page without passing an `id` or passes a wrong `id`, then your app must redirect them to a friendly error page.


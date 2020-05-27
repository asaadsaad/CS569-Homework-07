# CS569 Homework 08
### Angular Router Module and Guards
* Create a service `db` that returns an observable with the following response:
```javascript
[{_id: 1, name:'Natural Prairie', produce:['lettuce', 'tomato']}, ...]
```
* Add another method that returns an observable with full details of a single farm by `id`.
* Create a component `farmersMarket` that is responsible for showing a list of farm names.
```html
<ul>
  <li><a href="/farm/1">Natural Prairie</a></li>
  ...
</ul> 
```
* When users click on a farm name link you should direct them to a `farmDetails` child component that shows produce details of the farm.
* If a user tried to visit `farmDetails` page without passing an `id` or passes a wrong `id`, then your app will redirect them to a friendly error page.


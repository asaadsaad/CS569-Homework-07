# CS569 Homework 
Create an Angular application that uses the [Dog API](https://dog.ceo/dog-api/)
* Display a list of all breeds.
* When a breed is selected, display a list of all sub-breeds along with 3 random pictures of the selected breed.
* When a sub-breed is selected, display 3 random pictures of the selected sub-breed (consider using nested routes).
* Considering we have a list of banned breeds, maintained in a service, and persisted to the localStorage, add a button to each breed page to be added/removed to/from the banned list.
* Create a page to show all banned breeds.
* Create a guard that checks if the selected breed is added to the banned list, so it displays a [confirm alert](https://www.w3schools.com/jsref/met_win_confirm.asp) before it navigates to the breed page.
## Requests:
* List all breeds: `https://dog.ceo/api/breeds/list/all`
* List Sub-breeds: `https://dog.ceo/api/breed/{breed}/list`
* Breed image(n): `https://dog.ceo/api/breed/{breed}/images/random/{n}`
* Sub-breed image(n): `https://dog.ceo/api/breed/{breed}/{sub-breed}/images/random/{n}`
```typescript
export interface ListBreedsResponse {
    message: { [key: string]: any[]; };
    status: string;
}
export interface SubBreedResponse {
    message: string[];
    status: string;
}
export interface BreedImageResponse {
    message: string;
    status: string;
}
export interface SubBreedImageResponse {
    message: string;
    status: string;
}
```



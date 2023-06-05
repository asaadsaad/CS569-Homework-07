# CS569 Homework
### Angular Router Module and Guards
**Update the previous Homework:**
  
* Import Angular Router module
* Remove the Show/Hide button and convert `AppComponent` into a template displaying the `ListComponent` component when `/` is requested.
* Create a guard to enforce the user on using Google Chrome browser, if not, a friendly error page should be displayed. You may use the following service:
```typescript
import { Injectable } from '@angular/core';

@Injectable({
  providedIn: 'root'
})
export class BrowserDetector {
  isChrome() {
    return navigator.userAgent.indexOf('Chrome') > -1;
  }
}
```
* Given a list of the following nationalities:
```typescript
nationalities : string[] = ['AU', 'BR', 'CA', 'CH', 'DE', 'DK', 'ES', 'FI', 'FR', 'GB', 'IE', 'IN', 'IR', 'MX', 'NL', 'NO', 'NZ', 'RS', 'TR', 'UA', 'US']
```
Create router links on `AppComponent` as follows: `Filter by: AU, BR, CA ...etc`, each one sends a request to the following URL: `https://randomuser.me/api/?results=10&nat=US` (replace the query parameter with the nationality code). When a nationality is selected, display a message: `Showing users from the US` and provide a link to remove the filter.



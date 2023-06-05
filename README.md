# CS569 Homework
### Angular Router Module and Guards
**Update the previous Homework:**
  
* Add Angular Router module
* Remove the Show/Hide button and convert `AppComponent` into a template with a router link to navigate to `ListComponent` when `/list` is requested.  =
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
**Extra Requirements:**
  
Given a list of the following nationalities:
```typescript
nationalities : string[] = ['AU', 'BR', 'CA', 'CH', 'DE', 'DK', 'ES', 'FI', 'FR', 'GB', 'IE', 'IN', 'IR', 'MX', 'NL', 'NO', 'NZ', 'RS', 'TR', 'UA', 'US']
```
Create router links on `AppComponent`, each one sends a request to the following URL: `https://randomuser.me/api/?results=10&nat=US` (replace the query parameter with the nationality code). When a nationality is selected, display a message: `Showing users from the US`.



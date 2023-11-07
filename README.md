# CS569 Homework
**Update the previous Homework:**
  
* Import Angular Router module
* Remove the Show/Hide button and convert `AppComponent` into a template (use a router outlet) displaying the `ListComponent` component when `/` is requested.
* Create a guard to force the user to use Google Chrome browser, if not, a friendly error page should be displayed. You may use the following service:
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
Display router links on `ListComponent` as follows: `Filter by: AU, BR, CA ...etc`, each nationality is a link that sends a request to the following URL: `https://randomuser.me/api/?results=10&nat=US` (replace the query parameter with the nationality code). When a nationality link is clicked, display a message: `Filtered by: US` and an <ins>(remove filter)</ins> link to remove the filter.



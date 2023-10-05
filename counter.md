home.page.html
```html
<ion-content [fullscreen]="true">
<div id="counter">
  <h1>Count: {{ counter}}></h1>
<ion-button shape = "round" (click) = "increase()">Increase</ion-button>
</div>
</ion-content>
```


hoome.page.ts
```js
import { Component } from '@angular/core';

@Component({
  selector: 'app-home',
  templateUrl: 'home.page.html',
  styleUrls: ['home.page.scss'],
})

export class HomePage {
counter = 0;

increase(){
this.counter++;
}

constructor(){ }

}
```
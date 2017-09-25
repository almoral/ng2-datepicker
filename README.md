# mdc-date
Angular2 Datepicker Component

***mdc-date*** is a datepicker component for Angular2.

## Installation:

Install mdc-date via `npm`

````shell
npm install mdc-date --save
````

## Integration

```ts
// app.module.ts
import { DatePickerModule } from 'ng2-datepicker';

@NgModule({
  ...
  imports: [ DatePickerModule ]
  ...
})
export class AppModule { }

// app.component.ts
import { Component } from '@angular/core';
import { DatePickerOptions, DateModel } from 'ng2-datepicker';

@Component({
  selector: 'app-root',
  templateUrl: 'app.component.html'
})
export class AppComponent {
  date: DateModel;
  options: DatePickerOptions;

  constructor() {
    this.options = new DatePickerOptions();
  }
}

// app.component.html
<ng2-datepicker [options]="options" [(ngModel)]="date"></ng2-datepicker>
```

## AoT Library Build

```shell
npm run build:lib
```

## Licence

This project is licensed under the MIT license. See the [LICENSE](LICENSE) file for more info.

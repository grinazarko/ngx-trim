# ngx-trim

## Installation

To install this library, run:

```bash
$ npm install ngx-trim --save
```

## Consuming your library

Once you have published your library to npm, you can import your library in any Angular application by running:

```bash
$ npm install ngx-trim
```

and then from your Angular `AppModule`:

```typescript
import { BrowserModule } from '@angular/platform-browser';
import { NgModule } from '@angular/core';

import { AppComponent } from './app.component';
// Import the library
import { NgxTrimModule } from 'ngx-trim';

@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule,
// Import the library    
    NgxTrimModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }
```

Once your library is imported, you can use its components, directives and pipes in your Angular application:

```xml
<!-- You can now use your library component in app.component.html -->

<input type="text"  placeholder="input" [(ngModel)]="testInput" ngxTrim>

```

## Development

To generate all `*.js`, `*.d.ts` and `*.metadata.json` files:

```bash
$ npm run build
```

To lint all `*.ts` files:

```bash
$ npm run lint
```

## License

MIT © [Sam Lin](mailto:maxisam@gmail.com)
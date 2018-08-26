# Link a paginas

app.modules.ts
```
import { EjemploPage } from '../pages/ejemplo/ejemplo';

declarations: [
    EjemploPage,
  ],
  
 entryComponents: [
    EjemploPage,
  ],
```

home.ts
```
import { EjemploPage } from '../ejemplo/ejemplo';
export class HomePage {
  ejemploPage = EjemploPage;
  constructor(public navCtrl: NavController) {}
```

home.html
```
<button ion-button block color="mycolor" [navPush]="ejemploPage">Vamos a Ejemplo</button>
```

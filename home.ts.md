# Mostrar un Log

```
console.log('Saved clicked');
```

# Mostrar Lista

```
public todos: any[];

constructor(public navCtrl: NavController, public navParams: NavParams) {
  }

  ionViewDidLoad() {
    this.todos = [
      {
        descriptions: "esto es una tarea",
        isDone: false
      }
    ]
  }
  
  
```

```
<ion-content padding>
    <ion-list>
      <ion-item *ngFor="let todo of todos">
        {{todo.descriptions}}
      </ion-item>
    </ion-list>
</ion-content>  
  
```

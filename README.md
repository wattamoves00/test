# test

<ion-content padding>
      <ion-item>
    <ion-label floating>name</ion-label>
    <ion-input [(ngModel)]="name1" type="text"></ion-input>
   

    
     </ion-item>
<button ion-button (click)="name(name1)"> Greet Me </button>


  name(){
    if( this.name1 == "randy" || this.name1 == "manuel")
   alert("Good afternoon " + this.name1);
  else if( this.name1 == "kenneth" || this.name1 == "rowell")
   alert("Good Night " + this.name1!!);
  else
  alert("Your name is steven..")
 }
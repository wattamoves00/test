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
 
 
 ----------------------------------------------------------
 
 <ion-content padding>
      <ion-item>
    <ion-label floating>First Name</ion-label>
    <ion-input [(ngModel)]="name1" type="text"></ion-input>
      </ion-item>
      <ion-item>
    <ion-label floating>Second Name</ion-label>
    <ion-input [(ngModel)]="name2" type="text"></ion-input>

    
     </ion-item>
<button ion-button (click)="name()"> Greet Me </button>

 
 
  @Component({
  selector: 'page-home',
  templateUrl: 'home.html'
})

export class HomePage {
name1: string = '';
name2: string = '';
errorChk;
// title = 'Tour of Heroes';
// heroes = HEROES;
// selectedHero: Hero;
  
  //  onSelect(hero: Hero): void {
  //   this.selectedHero = hero;
  // }
  
  constructor(public navCtrl: NavController) {  }

  name(){
   if( this.name1 == '' && this.name2 == '') alert ('fill the form')
   else if( this.name1 === this.name2)
   alert("Good afternoon " + this.name1);
  else
  alert("Good night " + this.name1 + "  " + 
  "Good night " + this.name2);
 }

  
 
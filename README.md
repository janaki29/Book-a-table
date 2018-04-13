#include<cstdio>
#include<cstdlib>
#include<iostream>
using namespace std;
void display(){
	cout<<"\nNames of cafe are:\n";cout<<"\n1.Cafe Coffee Day\n"; cout<<"\n2.Coffee Corner\n"; cout<<"\n3.Meet n Melt \n";cout<<"\n4.Mickey Metro \n";cout<<"\n\n";
}

void display_(){
	int a;
	cout<<"\nEnter the Cafe number....\n";
	cout<<"\nAvailable Cafes are:\n";cout<<"\n1.Cafe Coffee Day\n"; cout<<"\n2.Coffee Corner\n"; cout<<"\n3.Meet n Melt \n";cout<<"\n4.Mickey Metro \n";cout<<"\n\n";
	 cin>>a;
	switch(a){
	case 1: cout<<"\n1.Cafe Coffee Day\n";
	        cout<<"\nAddress: Navathe, Amravati"; cout<<"\nContact: 9876543210\nEmail ID:ccd_amt@gmail.com\n\n";
	        break;
	case 2: cout<<"\n2.Coffee Corner\n"; 
	        cout<<"\nAddress:Gopal Nagar, Amravati"; cout<<"\nContact: 9876543210\nEmail ID:cornerCoffee@gmail.com\n\n";
	        break;
	case 3: cout<<"\n3.Meet n Melt \n";
	        cout<<"\nAddress: Dastur Nagar, Amravati"; cout<<"\nContact: 9876543210\nEmail ID:meetNmelt@gmail.com\n\n";
	        break;
	case 4: cout<<"\n4.Mickey Metro  \n";cout<<"\n\n";
		    cout<<"\nAddress: Saturna, Amravati"; cout<<"\nContact: 9876543210\nEmail ID:mickeyMetro_mm@gmail.com\n\n";
	        break;
	default: cout<<"\n!!!!\nYou can select only those choices which are given above....Please try again\n\n\n";
	}
}

void add_name(){
	cout<<"To add your name to the list of Cafes Please contact on the number given below....\nJanaki Dehankar\nMobile no.:+91-9876543210\nEmail ID:dehankarjanaki@gmail.com"<<endl;
}

void ccd(){int n;
	cout<<"\n Only 20 tables are available....\nOut of which u can book table which are indicated by E indicating Empty whereas R indicate Reserved....\n";
	char array[20];
	for(int i=0;i<20;i++)
	array[i]='E';
		for(int i=0;i<20;i++){
	    if(i%5==0)cout<<endl;
	    if(i>8) cout<<i+1<<"."<<array[i]<<"\t";
	    else cout<<i+1<<"."<<array[i]<<"\t\t";
	}
	cout<<"\n\nEnter table number u wanna book....\n\t\t\t\t"; cin>>n;
	array[n-1]='R';
	cout<<"\nTables after ur booking....\n";
	for(int i=0;i<20;i++){
	    if(i%5==0)cout<<endl;
	    cout<<i+1<<"."<<array[i]<<"\t\t";
	}
	cout<<endl; 	cout<<endl;  	cout<<endl;
}

void corner_cafe(){
   int n;
   cout<<"\n27 tables are available....\nOut of which u can book table which are indicated by E indicating Empty whereas R indicate Reserved....\n";
	char array[27];
	for(int i=0;i<27;i++)
	array[i]='E';
		for(int i=0;i<27;i++){
	    if(i%3==0)cout<<endl;
	    if(i>8) cout<<i+1<<"."<<array[i]<<"\t";
	    else cout<<i+1<<"."<<array[i]<<"\t\t";
	}
	cout<<"\n\nEnter table number u wanna book....\n\t\t\t\t"; cin>>n;
	if(n>27) cout<<"!!!!....Please enter table numbers between 1 & 27....Try again\n";
	else { array[n-1]='R';
	cout<<"\nTables after ur booking....\n";
	for(int i=0;i<27;i++){
	    if(i%3==0)cout<<endl;
	    if(i>8) cout<<i+1<<"."<<array[i]<<"\t";
	    else cout<<i+1<<"."<<array[i]<<"\t\t";
	}
	cout<<endl; 	cout<<endl;  	cout<<endl;
	}
}

void meetNmelt(){
     int n;
    cout<<"\nWelcome to Meet N Melt....\n";
   cout<<"\n40 tables are available....\nOut of which u can book table which are indicated by E indicating Empty whereas R indicate Reserved....\n";
	char array[40];
	for(int i=0;i<40;i++)
	array[i]='E';
		for(int i=0;i<40;i++){
	    if(i%4==0)cout<<endl;
	    if(i>8) cout<<i+1<<"."<<array[i]<<"\t";
	    else cout<<i+1<<"."<<array[i]<<"\t\t";
	}
	cout<<"\n\nEnter table number u wanna book....\n\t\t\t\t"; cin>>n;
	if(n>40) cout<<"!!!!....Please enter table numbers between 1 & 40....Try again\n";
	else { array[n-1]='R';
	cout<<"\nTables after ur booking....\n";
	for(int i=0;i<40;i++){
	    if(i%4==0)cout<<endl;
	    if(i>8) cout<<i+1<<"."<<array[i]<<"\t";
	    else cout<<i+1<<"."<<array[i]<<"\t\t";
	}
	cout<<endl; 	cout<<endl;  	cout<<endl;
	}
}

void mickeyMetro(){int n;
   cout<<"\n100 tables are available....\nOut of which u can book table which are indicated by E indicating Empty whereas R indicate Reserved....\n";
	cout<<"\nFirst 20 tables are for special celebrations....\n";
	char array[100];
	for(int i=0;i<100;i++)
	array[i]='E';
		for(int i=0;i<100;i++){
	    if(i%10==0)cout<<endl;
	    if(i>8) cout<<i+1<<"."<<array[i]<<"\t";
	    else cout<<i+1<<"."<<array[i]<<"\t\t";
	    if(i==19)cout<<"\n\n";
	}
	cout<<"\n\nEnter table number u wanna book....\n\t\t\t\t"; cin>>n;
	if(n>100) cout<<"!!!!....Please enter table numbers between 1 & 100....Try again\n";
	else { array[n-1]='R';
	cout<<"\nTables after ur booking....\n";
	for(int i=0;i<100;i++){
	    if(i%10==0)cout<<endl;
	    if(i>8) cout<<i+1<<"."<<array[i]<<"\t";
	    else cout<<i+1<<"."<<array[i]<<"\t\t";
	}
	cout<<endl; 	cout<<endl;  	cout<<endl;
	}
}

void reserve(){
	int c;
	cout<<"\nEnter the name of Cafe where u wanna reserve table.....\n";
	cout<<"\n1.Cafe Coffee Day\n"; cout<<"\n2.Coffee Corner\n"; cout<<"\n3.Meet n Melt \n";cout<<"\n4.Mickey Metro \n";cout<<"\n\n";
    cin>>c;
	switch(c){
		case 1: ccd(); break;
		case 2: corner_cafe(); break;
		case 3: meetNmelt(); break;
		case 4: mickeyMetro(); break;
	}
}

int main(){
	int x;
	while(1){
cout<<"\nEnter any one....\n\n";
cout<<"\n1.Names of Cafe \n2.Information of Cafe \n3.Book a table \n4.Want to Add Cafe name to the list \n5.Exit\n\n";
cin>>x;
switch(x){
	case 1: display(); break;
	case 2: display_(); break;
	case 3: reserve(); break;
	case 4: add_name(); break;
	case 5: exit(0);
}
}
return 0;
}

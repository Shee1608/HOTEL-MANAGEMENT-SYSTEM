#include<iostream>
using namespace std;

int main()
{
    int quant;
    int choice;
//Quantity
    int Qrooms=0, Qpasta=0, Qnoodles=0, Qburgur=0, Qshake=0, Qchicken=0;
//food items sold   
    int Srooms=0, Spasta=0, Snoodles=0, Sburger=0, Sshake=0, Schicken=0;
//Total price of items
    int total_rooms=0, total_pasta=0, total_noodles=0, total_burger=0, total_shake=0, total_chicken=0;

cout<<"\n\t Quantity of items we have";
cout<<"\n Rooms available:";

cin>>Qrooms;

cout<<"\n Quantity of pasta :";
cin>>Qpasta;

cout<<"\n Quantity of noodles :";
cin>>Qnoodles;

cout<<"\n Quantity of burger :";
cin>>Qburgur;

cout<<"\n Quantity of shake :";
cin>>Qshake;

cout<<"\n Quantity of Chicken :";
cin>>Qchicken;

m:

cout<<"\n\t\t Please select the given menu options";
cout<<"\n\n1 Rooms";
cout<<"\n2 Pasta";
cout<<"\n3 noddles";
cout<<"\n4 burger";
cout<<"\n5 Shake";
cout<<"\n6 chicken";
cout<<"\n7 Information regarding sales and collection";
cout<<"\n8 Exit";

cout<<"\n\n Please enter your choice";
cin>>choice;

switch (choice)
{
    case 1:
    cout<<"\n\n Enter the number of rooms you want:";
    
    cin>>quant;
    if (Qrooms-Srooms >= quant)
    {
        Srooms= Srooms+quant;
        total_rooms= total_rooms+quant*1000;
        cout<<"\n\n\t\t"<<quant<<"Room/Rooms have been alloted to you!";
    }
    else
        
        cout<<"\n\t Only"<<Qrooms-Srooms<<"Rooms remaining in the hotel";
        break;

    case 2:
    cout<<"\n\n Enter the number of Pasta you want:";
    
    cin>>quant;
    if (Qpasta-Spasta >= quant)
    {
        Spasta= Spasta+quant;
        total_pasta= total_pasta+quant*120;
        cout<<"\n\n\t\t"<<quant<<"pasta have been ordered";
    }
    else
        
        cout<<"\n\t Only"<<Qpasta-Spasta<<"Pasta remaining in the hotel";
        break;

    case 3:
    cout<<"\n\n Enter the number of noodles you want:";
    
    cin>>quant;
    if (Qnoodles-Snoodles >= quant)
    {
        Snoodles= Snoodles+quant;
        total_noodles= total_noodles+quant*150;
        cout<<"\n\n\t\t"<<quant<<"Noodles have been Ordered";
    }
    else
        
        cout<<"\n\t Only"<<Qnoodles-Snoodles<<"Noodles remaining in the hotel";
        break;

    case 4:
    cout<<"\n\n Enter the number of burger you want:";
    
    cin>>quant;
    if (Qburgur-Sburger >= quant)
    {
        Sburger= Sburger+quant;
        total_burger= total_burger+quant*90;
        cout<<"\n\n\t\t"<<quant<<"Burger have been ordered";
    }
    else
        
        cout<<"\n\t Only"<<Qburgur-Sburger<<"Burger remaining in the hotel";
        break;

    case 5:
    cout<<"\n\n Enter the number of shake you want:";
    
    cin>>quant;
    if (Qshake-Sshake >= quant)
    {
        Sshake= Sshake+quant;
        total_shake= total_shake+quant*100;
        cout<<"\n\n\t\t"<<quant<<"Shakes have been ordered";
    }
    else
        
        cout<<"\n\t Only"<<Qshake-Sshake<<"Shakes remaining in the hotel";
        break;

    case 6:
    cout<<"\n\n Enter the number of Chicken you want:";
    
    cin>>quant;
    if (Qchicken-Schicken >= quant)
    {
        Schicken= Schicken+quant;
        total_chicken= total_chicken+quant*250;
        cout<<"\n\n\t\t"<<quant<<"Chicken have been ordered";
    }
    else
        
        cout<<"\n\t Only"<<Qchicken-Schicken<<"Chicken remaining in the hotel";
        break;            
    break;

    case 7:

    cout<<"\n\tDetails of sales and collection";
    cout<<"\n\n Number of rooms we had: "<<Qrooms;
    cout<<"\n\n Number of rooms we gave for rent: "<<Srooms;
    cout<<"\nn Remaining rooms : "<<Qrooms-Srooms;
    cout<<"\n\n Total_rooms collection for the day : "<< total_rooms;

    cout<<"\n\n Number of pasta we had: "<<Qpasta;
    cout<<"\n\n Number of pasta we gave:  "<<Spasta;
    cout<<"\nn Remaining pasta : "<<Qpasta-Spasta;
    cout<<"\n\n Total_pasta collection for the day : "<< total_pasta;
    
    cout<<"\n\n Number of noodles we had: "<<Qnoodles;
    cout<<"\n\n Number of noodles we gave: "<<Snoodles;
    cout<<"\nn Remaining noodles : "<<Qnoodles-Snoodles;
    cout<<"\n\n Total_noodles collection for the day : "<< total_noodles;
    
    cout<<"\n\n Number of burger we had: "<<Qburgur;
    cout<<"\n\n Number of burger we gave: "<<Sburger;
    cout<<"\nn Remaining burger : "<<Qburgur-Sburger;
    cout<<"\n\n Total_burger collection for the day : "<< total_burger;
    
    cout<<"\n\n Number of shake we had: "<<Qshake;
    cout<<"\n\n Number of shake we gave: "<<Sshake;
    cout<<"\nn Remaining shake: "<<Qshake-Sshake;
    cout<<"\n\n Total_shake collection for the day : "<< total_shake;
    
    cout<<"\n\n Number of chicken we had: "<<Qchicken;
    cout<<"\n\n Number of chicken we gave: "<<Schicken;
    cout<<"\nn Remaining Shake : "<<Qchicken-Schicken;
    cout<<"\n\n Total_shake collection for the day : "<< total_shake;


    cout<<"\n\n Total collection for a day:"<< total_rooms + total_burger + total_chicken + total_noodles + total_pasta + total_shake;
    break;
    
    case 8:
        exit(0);

default:
    cout<<"\n Please select the numbers mentioned above!";
   }

goto m;
}








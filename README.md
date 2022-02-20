# currency_converter
One of the best ways to revise basic concepts is to build a basic project, and there’s nothing easier than a converter. All you have to do is take input of the currency required and display the output accordingly. There also needs to be a way to customize the currencies from some sort of menu or dropdown. Data for the conversion can be fetched from an external file, or simply stored as a separate module.A converter should have some validation to ensure that the conversion works only on numeric data. An error should be displayed for invalid data accordingly.
code-
#include<iostream>
using namespace std;
int main() {
int opt1,opt2;
double amount;
cout<<"****Welcome To the Currency Converter Application****"<<endl;
cout<<"****Choose Any Currency You Want To Convert****"<<endl;
cout<<"1.)Indian Rupees "<<endl;
cout<<"2.)American Dollars "<<endl;
cout<<"3.)Japanese Yen "<<endl;
cout<<"4.)Euro "<<endl;
cout<<"5.)British Pounds"<<endl;
cout<<"Please Enter Your Choice No Here : "<<endl;
cin>>opt1;
cout<<"Please Enter The Amount You Want To Convert : "<<endl;
cin>>amount;


cout<<"****please Select The Currency In Which You Want To Convert In**** "<<endl;
cout<<"1.)Indian Rupees "<<endl;
cout<<"2.)American Dollars "<<endl;
cout<<"3.)Japanese Yen "<<endl;
cout<<"4.)Euro "<<endl;
cout<<"5.)British Pounds"<<endl;
cout<<"Please Enter Your Choice No Here : "<<endl;
cin>>opt2;

switch (opt1)
{
case 1:
    switch (opt2)
    {
    case 1:cout<<"No Change "<<endl;   //indian rupees to indian rupees
           cout<<"Amount : "<<amount<<endl;  
           break;
    case 2: cout<<"Amount : "<<amount*0.013<<endl;           //rupees to usd
           break;
    case 3:cout<<"Amount : "<<amount*1.54<<endl;                //rupees to yen
           break;
    case 4:cout<<"Amount : "<<amount*0.009<<endl;                //rupees to pound
           break;
    case 5:cout<<"Amount : "<<amount*0.011<<endl;                //rupees to euro
           break;
    }
    break;
case 2:
    switch (opt2)
    {
    case 1:cout<<"Amount : "<<amount*75.13<<endl; //usd to rupees
           break;
    case 2:cout<<"No change"<<endl;
           cout<<"Amount : "<<amount<<endl;           //usd to usd          
           break;
    case 3:cout<<"Amount : "<<amount*115.16<<endl;                //usd to yen                
           break;
    case 4:cout<<"Amount : "<<amount*0.73<<endl;               
           break;
    case 5:cout<<"Amount : "<<amount*0.86<<endl;                
           break;
    }
    break;
case 3:
    switch (opt2)
    {
    case 1:cout<<"Amount : "<<amount*0.64<<endl;    //yen to rupees
           break;
    case 2:cout<<"Amount : "<<amount*0.008<<endl;   //yen to usd
           break;
    case 3:cout<<"No change"<<endl;
           cout<<"Amount : "<<amount<<endl;                //yen to yen
           break;
    case 4:cout<<"Amount : "<<amount*0.006<<endl;                //yen to pound
           break;
    case 5:cout<<"Amount : "<<amount*0.007<<endl;            //yen to euro
           break;
    }
    break;
case 4:
    switch (opt2)
    {
    case 1:cout<<"Amount : "<<amount*101.54<<endl;   //pounds to rupees
           break;
    case 2:cout<<"Amount : "<<amount*1.36<<endl;     //pounds to usd
           break;
    case 3:cout<<"Amount : "<<amount*156.64<<endl;    //pounds to yen
           break;
    case 4:cout<<"No change"<<endl;
           cout<<"Amount : "<<amount<<endl;                //pounds to pound
           break;
    case 5:cout<<"Amount : "<<amount*1.19<<endl;                //pounds to euro
           break;
    }
    break;  
case 5:
    switch (opt2)
    {
    case 1:cout<<"Amount : "<<amount*84.75<<endl;  //euro to rupees
           break;
    case 2:cout<<"Amount : "<<amount*1.13<<endl;           //euro to usd
           break;
    case 3:cout<<"Amount : "<<amount*130.85<<endl;                //euro to yen
           break;
    case 4:cout<<"Amount : "<<amount*0.83<<endl;                //euro to pound
           break;
    case 5:cout<<"No change"<<endl;
           cout<<"Amount : "<<amount<<endl;                //euro to euro
           break;
    }
    break;  
//     cout<<"Thankyou,For Using our service :) "<<endl;   
}
cout<<"Thankyou!! For Using our service :) "<<endl;
return 0;
}
  

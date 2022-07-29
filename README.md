#include <iostream>

using namespace std;

enum encolor { red=100 , green=200 , white=300 , black=400 };
enum engendor { male=2 , female=1 };
enum enmarried { yes=1 , no=0 };

struct sthowami{
    
   
    string monthlysalary;
    string anythink;
    
};

struct stadrries{
    
    string city;
    string country;
    sthowami my;
};

struct stdatainfo{
    
    stadrries finaly;
    encolor color;
    engendor gendor;
    enmarried married;
     string name;
    string age;
    
};
int main()
{
   
   stdatainfo person1;
   
   person1.name="Mhamad Hussain";
   person1.age="23";
   
   person1.finaly.city="AL-NAJAF";
    person1.finaly.country="al-iraq";
    person1.finaly.my.monthlysalary="50000 dinar iraqy";
     person1.finaly.my.anythink="hello world";
    
    person1.color=encolor::green;
    person1.gendor=engendor::male;
   person1.married=enmarried::no;
   
   cout<<"name= " <<person1.name<<endl;
   cout<< "age= " <<person1.age<<endl;
   
   cout<<"city= " <<person1.finaly.city<<endl;
   cout<<"country= " <<person1.finaly.country<<endl;
   cout<<"monthlysalary= " <<person1.finaly.my.monthlysalary<<endl;
   cout<<"anythink= " <<person1.finaly.my.anythink<<endl;
   
   cout<<"my color= "<< person1.color<<endl;
   cout<< "my gonder= "<< person1.gendor<<endl;
   cout<< "my married= "<< person1.married<<endl;
   

    return 0;
}
